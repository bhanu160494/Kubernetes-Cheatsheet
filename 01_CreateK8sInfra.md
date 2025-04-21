# Install kubectl

## Pre-requisite: 
- Download and install docker desktop
- Download and install chocolatey package manager (choco)
  * Package manager for windows(powershell) that allows to install, update and manage S/W packages.
  * Package mananger for linux are APT, YUM, DNF etc.
- Install curl

  ```choco install curl -y```

## Download the latest release of kubectl
```sh
curl.exe -LO "https://dl.k8s.io/release/v1.32.0/bin/windows/amd64/kubectl.exe"
```

## Add the binary to your PATH
```sh
move kubectl.exe C:\Windows\System32
```

## Verify the installation
```sh
kubectl version --client
kubectl version
```

## Install minikube

**download the latest release of minikube**
```sh
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-installer.exe)
```

**Run the installer and verify the status**
```sh
minikube version
minikube status
minikube start
minikube stop
```
