# My Music App with Kubernetes ⎈

This is my local music app with folders/playlists systems running with **Kubernetes** and **PHP**.

## Prerequisites

Before you start, make sure you have the following tools installed:

- Docker
- Kind (Kubernetes in Docker)
- Git

If you don't have these tools yet, you can follow the official documentation for each one to install them.

## Installation Steps

Follow the steps below to set up and run the app locally:

```bash
#Clone repository and chose them
git clone https://github.com/andradesysadmin/mymp3-kubernets
cd mymp-kubernets

#Create kind cluster and apply the manifests
kind create cluster --config kind/kind-config.yaml
kubectl apply -f manifests/

```
After this, you can acess the aplication with the node worker IP in 30080 port, some like this:

```
http://172.19.0.4:30080/

```
**Note**: The worker node IP may vary depending on your environment. Use the command *kubectl get nodes -o wide* to get the correct IP.

