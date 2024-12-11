# DO droplet
(https://docs.digitalocean.com/products/droplets/getting-started/recommended-droplet-setup/)
```bash
$ doctl auth init --context <projectname> # this will need a token generated in (https://cloud.digitalocean.com/account/api/tokens)
# doctl installed with snap
$ sudo snap connect doctl:ssh-keys :ssh-keys
$ sudo snap connect doctl:kube-config # to give kubectl access
# When you set up Digital Ocean you gave your ssh key a name keyname
$ doctl compute ssh-key import <keyname> --public-key-file ~/.ssh/id_rsa.pub
# If things are set up correctly this will error with "SSH Key is already in use on your account"



```

### cloudconfig.sh script
```
#!/bin/bash
set -euo pipefail

USERNAME=<username> # TODO: Customize the sudo non-root username here

# Create user and immediately expire password to force a change on login
useradd --create-home --shell "/bin/bash" --groups sudo "${USERNAME}"
passwd --delete "${USERNAME}"
chage --lastday 0 "${USERNAME}"

# Create SSH directory for sudo user and move keys over
home_directory="$(eval echo ~${USERNAME})"
mkdir --parents "${home_directory}/.ssh"
cp /root/.ssh/authorized_keys "${home_directory}/.ssh"
chmod 0700 "${home_directory}/.ssh"
chmod 0600 "${home_directory}/.ssh/authorized_keys"
chown --recursive "${USERNAME}":"${USERNAME}" "${home_directory}/.ssh"

# Disable root SSH login with password
sed --in-place 's/^PermitRootLogin.*/PermitRootLogin prohibit-password/g' /etc/ssh/sshd_config
# this won't work on ubuntu, the service is ssh
if sshd -t -q; then systemctl restart sshd; fi 

```