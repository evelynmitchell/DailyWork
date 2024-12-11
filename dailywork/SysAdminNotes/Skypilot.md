# Skypilot
```
# NOTE: '--platform linux/amd64' is needed for Apple silicon Macs
docker run --platform linux/amd64 \
  -td --rm --name sky \
  -v "$HOME/.sky:/root/.sky:rw" \
  -v "$HOME/.aws:/root/.aws:rw" \
  -v "$HOME/.config/gcloud:/root/.config/gcloud:rw" \
  berkeleyskypilot/skypilot

docker exec -it sky /bin/bash
```

```
(base) root@f5394a39356a:/# sky local up
SkyPilot collects usage data to improve its services. `setup` and `run` commands are not collected to ensure privacy.
Usage logging can be disabled by setting the environment variable SKYPILOT_DISABLE_USAGE_COLLECTION=1.
Creating local cluster...
To view detailed progress: tail -n100 -f ~/sky_logs/sky-2024-12-10-19-55-14-228905/local_up.log
RuntimeError: Failed to create local cluster. Full log: ~/sky_logs/sky-2024-12-10-19-55-14-228905/local_up.log
Error: Some dependencies were not found or are not configured correctly. Please fix the following errors and try again:

* Docker is not running. Please start Docker and try again.

* kind is not installed. Please install kind and try again.
Installation instructions: https://kind.sigs.k8s.io/docs/user/quick-start/#installation

* kubectl is not installed. Please install kubectl and try again.
Installation instructions: https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

```

```
(base) root@f5394a39356a:/# more ~/sky_logs/sky-2024-12-10-19-55-14-228905/local_up.log
Some dependencies were not found or are not configured correctly. Please fix the
 following errors and try again:

* Docker is not running. Please start Docker and try again.

* kind is not installed. Please install kind and try again.
Installation instructions: https://kind.sigs.k8s.io/docs/user/quick-start/#insta
llation

* kubectl is not installed. Please install kubectl and try again.
Installation instructions: https://kubernetes.io/docs/tasks/tools/install-kubect
l-linux/

```

## kind
```
#(https://kind.sigs.k8s.io/docs/user/quick-start/#installation)

[ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64

```
failed
```
(base) root@f5394a39356a:/# [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
bash: curl: command not found
```
running outside skypilot container
```
name:~$  [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
$ chmod +x ./kind
$ ./kind
```
Inside skypilot container
```
$ wget https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
$ mv kind-linux-amd64 ./kind
$ chmod +x kind 
$ ./kind
kind creates and manages local Kubernetes clusters using Docker container 'nodes'

Usage:
  kind [command]

Available Commands:
  build       Build one of [node-image]
  completion  Output shell completion code for the specified shell (bash, zsh or fish)
  create      Creates one of [cluster]
  delete      Deletes one of [cluster]
  export      Exports one of [kubeconfig, logs]
  get         Gets one of [clusters, nodes, kubeconfig]
  help        Help about any command
  load        Loads images into nodes
  version     Prints the kind CLI version

Flags:
  -h, --help              help for kind
      --loglevel string   DEPRECATED: see -v instead
  -q, --quiet             silence all stderr output
  -v, --verbosity int32   info log verbosity, higher value produces more output
      --version           version for kind

Use "kind [command] --help" for more information about a command.

```
## kubectl
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```
(https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)
Using wget within skypilot container
```
$ wget https://dl.k8s.io/release/v1.31.4/bin/linux/amd64/kubectl
$ chmod +x kubectl
$ ./kubectl
./kubectl 
kubectl controls the Kubernetes cluster manager.

 Find more information at: https://kubernetes.io/docs/reference/kubectl/

Basic Commands (Beginner):
  create          Create a resource from a file or from stdin
  expose          Take a replication controller, service, deployment or pod and
expose it as a new Kubernetes service
  run             Run a particular image on the cluster
  set             Set specific features on objects

Basic Commands (Intermediate):
  explain         Get documentation for a resource
  get             Display one or many resources
  edit            Edit a resource on the server
  delete          Delete resources by file names, stdin, resources and names, or
by resources and label selector

Deploy Commands:
  rollout         Manage the rollout of a resource
  scale           Set a new size for a deployment, replica set, or replication
controller
  autoscale       Auto-scale a deployment, replica set, stateful set, or
replication controller

Cluster Management Commands:
  certificate     Modify certificate resources
  cluster-info    Display cluster information
  top             Display resource (CPU/memory) usage
  cordon          Mark node as unschedulable
  uncordon        Mark node as schedulable
  drain           Drain node in preparation for maintenance
  taint           Update the taints on one or more nodes

Troubleshooting and Debugging Commands:
  describe        Show details of a specific resource or group of resources
  logs            Print the logs for a container in a pod
  attach          Attach to a running container
  exec            Execute a command in a container
  port-forward    Forward one or more local ports to a pod
  proxy           Run a proxy to the Kubernetes API server
  cp              Copy files and directories to and from containers
  auth            Inspect authorization
  debug           Create debugging sessions for troubleshooting workloads and
nodes
  events          List events

Advanced Commands:
  diff            Diff the live version against a would-be applied version
  apply           Apply a configuration to a resource by file name or stdin
  patch           Update fields of a resource
  replace         Replace a resource by file name or stdin
  wait            Experimental: Wait for a specific condition on one or many
resources
  kustomize       Build a kustomization target from a directory or URL

Settings Commands:
  label           Update the labels on a resource
  annotate        Update the annotations on a resource
  completion      Output shell completion code for the specified shell (bash,
zsh, fish, or powershell)

Subcommands provided by plugins:

Other Commands:
  api-resources   Print the supported API resources on the server
  api-versions    Print the supported API versions on the server, in the form of
"group/version"
  config          Modify kubeconfig files
  plugin          Provides utilities for interacting with plugins
  version         Print the client and server version information

Usage:
  kubectl [flags] [options]

Use "kubectl <command> --help" for more information about a given command.
Use "kubectl options" for a list of global command-line options (applies to all
commands).
```

## docker
(https://docs.docker.com/engine/install/binaries/)
(https://download.docker.com/linux/static/stable/x86_64/)
```
$ wget https://download.docker.com/linux/static/stable/x86_64/docker-27.4.0.tgz
$ tar xvzf docker-27.4.0.tgz 
docker/
docker/runc
docker/containerd
docker/docker-init
docker/dockerd
docker/containerd-shim-runc-v2
docker/docker-proxy
docker/docker
docker/ctr
$ cp docker/* /usr/bin/
$ cp kind /usr/bin/
$ cp kubectl /usr/bin/
```

```console
# start the docker daemon
$ dockerd &
```
