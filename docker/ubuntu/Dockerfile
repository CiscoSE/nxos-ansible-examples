# syntax=docker/dockerfile:1.4

FROM ubuntu:latest

ARG DEBIAN_FRONTEND=noninteractive

RUN <<EOF
apt update
apt upgrade -y
apt install ansible python3-pip vim git iputils-ping -y
pip3 install --upgrade pip
#pip3 install xmljson lxml pyopenssl jmespath
ansible-galaxy collection install cisco.aci
EOF
