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

## networking

https://docs.all-hands.dev/modules/usage/runtimes/docker#hardened-docker-installation

# Create an isolated network
docker network create openhands-network

# Run OpenHands in the isolated network
docker run # ... \
    --network openhands-network \
    
    
    


---
```
c2stYW50LWFwaTAzLTM2Nmt5SzR5RjV1RHNBUzlOTlVJQ2tLTHdGcXltZjFkdWJETDZCdkFSd1NR
TGZoTUJQbU9TR2hCbHJJcGg2dXgxWnFJbDFXUVlCeU1MbDFjUms0SWNnLTdvYW1ZQUFBCg==
QUl6YVN5QnVkaDRyMGZ1UlNWTVo0b3ZSelVtMVJ1bHRfT0pWdXY0Cg==
Z2l0aHViX3BhdF8xMUFBSFY3WlkwZWtyb0NBZGR2aXNsX2FjbVZxbEJ1Z3l4WHVHTEZ6WEZWYnlr
MDFtRVNCV0NHTWJWYTFMT2swSWxCVU40UllXRTQ3SW1zaUhQCg==
```
