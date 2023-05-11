# Container image infection

Collection of Dockerfile templates to be used in penetration tests and other red-teaming engagments, to seamlessly infect different types of container images with various reverse-shell backdoors.


# Metadata

| Repository type | State |
|---|---|
| Proof of Concept (PoC) | Unmaintained  |


# Background

During offensive engagments, it is not rare to compromise container registries, used as part of a deployment strategy. Since many companies tend to trust images hosted on private registries, seamlessly infecting them with backdoors connecting to an attacker-controlled location can be an efficient way to spread in a large-scale infrastructure such as Kubernetes.

The key to a stealthy infection is to be as silent as possible from a deployment and runtime perspective, by keeping the original behavior of the images unchanged after the infection. 

This repository contains Dockerfile templates to infect various types of container images with reverse-shell backdoors, without changing their original behavior once instantiated in containers.


# Features

## Supported container images

- Distrofull images based on:
  - Alpine Linux
  - Debian
  - Ubuntu
- Distroless images, made distrofull with:
  - Alpine Linux

## Supported reverse shells
 - netcat
 - socat


# Instructions

- Infecting [Distrofull](https://github.com/mnemonic-no/container-image-infection/tree/master/Distrofull) images
- Infecting [Distroless](https://github.com/mnemonic-no/container-image-infection/tree/master/Distroless) images
