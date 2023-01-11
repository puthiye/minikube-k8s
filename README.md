# minikube-k8s

- Install docker-

$ sudo dnf -y install dnf-plugins-core
$ sudo dnf config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo
$ sudo dnf install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y

$ sudo systemctl enable docker --now

$ sudo usermod -aG docker $USER
$ sudo newgrp docker

-Install minikube

$ curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
$ sudo install minikube-linux-amd64 /usr/local/bin/minikube

- Install kubectl

$ curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

$ chmod +x kubectl

$ sudo mv kubectl /usr/local/bin/


- Start minikube
- 
$ minikube start 

