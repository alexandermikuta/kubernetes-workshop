# Voraussetzungen

## Benötigte Installationen

- Virtualbox
- Docker (Alternativ: Podman)
- Kubernetes
- Kubectl
- Minikube
- Scaffold
- Lens
- Kompose

### Docker

### Kubernetes

### Kubectl

https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/

Installation mit:
  - curl: `curl.exe -LO "https://dl.k8s.io/release/v1.25.0/bin/windows/amd64/kubectl.exe"`
  - Choco: `choco install kubernetes-cli`
  - Scoop: `scoop install kubectl`
  - Winget: `winget install -e --id Kubernetes.kubectl`

Testen der Installation: `kubectl version --client`

### Minikube

https://minikube.sigs.k8s.io/docs/start/

Installation mit:
  - Powershell: ```New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing```
  - Winget: winget install minikube
  - Choco: choco install minikube

Testen der Installation: `minikube start` (Dashboard unter: `minikube dashboard`)

### Scaffold

### Lens

### Kompose

https://kompose.io/installation/
