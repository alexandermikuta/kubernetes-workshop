# Voraussetzungen

## Benötigte Installationen

- Docker
- Kubernetes
- Kubectl
- Minikube
- Helm
- Helmfile
- Skaffold
- Lens
- Kompose
- VSCode

### Docker

https://docs.docker.com/desktop/install/windows-install/

Zwei Installationsarten:
  - über WSL2: https://learn.microsoft.com/en-us/windows/wsl/install + Installation einer WSL2-Distro im Windows-Store, z.B. Ubuntu
  - Hyper-V (wird durch WSL2 ersetzt: https://www.docker.com/blog/docker-hearts-wsl-2/)

Empfehlungen:
  - In den Docker-Desktop-Settings den Speicher für Docker auf mindestens 8GB setzen
  - Windows-Terminal aus dem Windows-Store installieren

### Kubernetes

In Docker-Desktop aktivieren

Hinweis: Unter Windows sind Kubectl und Minikube bestandteil von Docker-Desktop!

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
  - Winget: `winget install minikube`
  - Choco: `choco install minikube`

Testen der Installation: `minikube start` (Dashboard unter: `minikube dashboard`)

### Helm

https://helm.sh/docs/intro/install/

Installation mit:
  - Choco: choco install kubernetes-helm
  - Scoop: scoop install helm

### Helmfile

https://helmfile.readthedocs.io/en/latest/#installation

Installation mit:
  - Scoop: scoop install helmfile

### Skaffold

https://skaffold.dev/docs/install/#standalone-binary

Installation mit:
  - Scoop: `scoop bucket add extras` und `scoop install skaffold`
  - Choco: `choco install -y skaffold`

### Lens

https://k8slens.dev/

### Kompose

https://kompose.io/installation/

Installation mit:
  - Choco: choco install kubernetes-kompose

### VSCode

https://code.visualstudio.com/

Empfohlene Plugins:
  - Cloud Code: https://marketplace.visualstudio.com/items?itemName=GoogleCloudTools.cloudcode
