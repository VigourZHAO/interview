Install Kubernetes: 
    Ref: https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

1. curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
2. curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
3. kubectl version --client
4. sudo apt-get update
5. sudo apt-get install -y apt-transport-https ca-certificates curl
6. sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg    【Failed】
    网页下载后手动 mv：sudo mv apt-key.gpg /usr/share/keyrings/kubernetes-archive-keyring.gpg
7. echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list       【Failed】
    修改：echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] http://mirrors.ustc.edu.cn/kubernetes/apt kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list

8. sudo apt-get install -y kubectl
9. kubectl version --client
10. kubectl cluster-info

Install minikube:
1. curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
2. sudo install minikube-linux-amd64 /usr/local/bin/minikube

