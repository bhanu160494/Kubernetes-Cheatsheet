# Install kubectl

## Download the latest release of kubectl
```sh
curl -LO "https://dl.k8s.io/release/$(curl -s https://dl.k8s.io/release/stable.txt)/bin/windows/amd64/kubectl.exe"
```

## Add the binary to your PATH
```sh
move kubectl.exe C:\Windows\System32
```

## Verify the installation
- kubectl version --client
- kubectl version

# Install docker desktop

# Install minikube

**download the latest release of minikube**
[Link](curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-installer.exe)

**Run the installer and verify the status**
minikube version
minikube status
minikube start
minikube stop
