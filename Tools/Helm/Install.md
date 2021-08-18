Download:
    Ref: https://helm.sh/zh/docs/intro/install/

Install:
1. curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -
2. sudo apt-get install apt-transport-https --yes
3. echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
4. sudo apt-get update
5. sudo apt-get install helm

命令行补充：
1. source <(helm completion bash)
2. helm completion bash > /etc/bash_completion.d/helm
