# docker-machine / compose migration

## Setup the server
### OS
OVH with custom kernel doesn't work:
`Error starting daemon: error initializing graphdriver: driver not supported`

Ubuntu 16.04 with original kernel work.

### docker-machine
First, be sure to create an account that has sudo access without password.

Run:
```bash
docker-machine create \
  --driver generic \
  --generic-ip-address=91.121.169.170 \
  --generic-ssh-user root \
  --generic-ssh-key ~/.ssh/id_rsa_cnode \
  kimsufi
```
