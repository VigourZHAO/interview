# Install Tools
sudo apt-get install subversion
sudo apt-get install docker.io
sudo apt-get install python3-pip
sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo usermod -aG docker ${USER}
sudo systemctl start docker
pip3 install sphinx

svn co Repo
cd firstquadrant/fq-deploy/
sh dev-web-service.sh

ERROR: Fix
    cd /root/firstquadrant/fq-images/fq-fl-baseimage/docker/dev
    sh build.sh 0.4
    cd /root/firstquadrant/fq-deploy
    sh dev-web-service.sh
    
    
prod
1. cd /home/zpx/SVN_Repo/firstquadrant/fq-webs/fqweb-server/docker/prod
2. vi fqweb/Dockerfile
3. docker-compose -f site-server.prod.yml builed up -d
4. 
5. docker exec -it prod_web sh
6.  
