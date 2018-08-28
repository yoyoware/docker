

<h1>install docker (https://get.docker.com)</h1>
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04

sudo apt update;sudo apt install apt-transport-https ca-certificates curl software-properties-common;curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -;sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable";sudo apt update;apt-cache policy docker-ce;sudo apt install docker-ce






sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install -y docker-compose;sudo docker run hello-world<br>
OR<br>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install docker-compose;sudo usermod -aG docker $(whoami)<br>
logout<br>
docker run hello-world<br>
<br>


<h1>install docker (https://get.docker.com)</h1>
sudo curl -L https://github.com/docker/compose/releases/download/1.18.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose;sudo chmod +x /usr/local/bin/docker-compose;docker-compose --version



sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install -y docker-compose;sudo docker run hello-world<br>
OR<br>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install docker-compose;sudo usermod -aG docker $(whoami)<br>
logout<br>
docker run hello-world<br>
<br>



<h1>install docker (https://docs.docker.com/compose/install)</h1>
sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose;sudo chmod +x /usr/local/bin/docker-compose


