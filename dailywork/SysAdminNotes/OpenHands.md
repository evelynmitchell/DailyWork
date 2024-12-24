## Install
[install](https://docs.all-hands.dev/)



```bash
docker pull docker.all-hands.dev/all-hands-ai/runtime:0.16-nikolaik

docker run -it --rm --pull=always \
    -e SANDBOX_RUNTIME_CONTAINER_IMAGE=docker.all-hands.dev/all-hands-ai/runtime:0.16-nikolaik \
    -e LOG_ALL_EVENTS=true \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -p 3000:3000 \
    --add-host host.docker.internal:host-gateway \
    --name openhands-app \
    docker.all-hands.dev/all-hands-ai/openhands:0.16
```

New claude key
https://docs.all-hands.dev/modules/usage/getting-started

![[Pasted image 20241220111108.png]]
