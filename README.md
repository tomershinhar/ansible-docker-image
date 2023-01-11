# ansible-docker-image

## Overview

this is a Dockerfile for building an image with ansible


## How to use
start by cloneing this repo.

then copy/move the playbooks you want to test to the `testing-playbooks` folder.

build the continer image using docker/podman

```bash
docker build -t {image-name} .  
```

run the continer
```bash
docker run -it {image-name} bash
```

all the playbooks that were passed to the `testing-playbooks` folder will now be under `/playbooks` folder and you can run them to verify that they are working correctly 

```bash
cd /playbooks
ansible-playbook (playbook-name}
```

