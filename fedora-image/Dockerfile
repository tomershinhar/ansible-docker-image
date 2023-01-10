
FROM registry.fedoraproject.org/fedora:latest
LABEL maintainer="tshinhar@redhat.com"

RUN mkdir /playbooks

RUN dnf update -y && \
    dnf install pip -y

RUN pip install ansible

COPY testing-playbooks /playbooks
