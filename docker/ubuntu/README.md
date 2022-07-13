To use this, run a docker build using buildkit. This will install ansible on an ubuntu image with support for the NXOS with Ansible.
```
buildkit=1 docker build -t ubuntu/ansible:v1 .
```
Something like the following can be used to map your source code into the docker container, or you can skip the -v portion of this and just use git to pull the repository to the docker image:
```
docker run --name ubuntu-ansible -it -v /path/to/demoCode/on/your/host/docker/system:/demo ubuntu/ansible:v1
```
