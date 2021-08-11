基础配置：
    1. Chrome:
        Step 1: echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" > /etc/apt/sources.list.d/google-chrome.list
        Step 2: sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 1397BC53640DB551
        Step 3: sudo apt update
        Step 4: sudo apt install google-chrome-stable
    2. SSH:
        1. ssh-keygen -t rsa -C "email"
    3. Git:
        1. Install:
            sudo apt install git
        2. Config Edit:
            git config --global core.editor "vim"
            git config --global user.email "you@example.com"
            git config --global user.name "Your Name"
    4. Curl:
        sudo apt install curl
    5. FQ:
        1. Install:
            v2ray-linux-64.zip
            Qv2ray.v2.6.3.linux-x64.AppImage
        2. Config:
            chmod +x Qv2ray.v2.6.3.linux-x64.AppImage

