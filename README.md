# my music app with kubernets 

This is my kubernets music app with PHP

## Steps to install
Install Docker, Kind, Git and run it: 
```bash
git clone https://github.com/andradesysadmin/mymp3-kubernets
cd mymp-kubernets
kind create cluster --config kind/kind-config.yaml
kubectl apply -f manifests/

```
