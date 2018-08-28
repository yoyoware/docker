

<h1>install docker (https://get.docker.com)</h1>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install -y docker-compose;sudo docker run hello-world<br>
OR<br>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install docker-compose;sudo usermod -aG docker $(whoami)<br>
logout<br>
docker run hello-world<br>
<br>


<h1>install docker (https://get.docker.com)</h1>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install -y docker-compose;sudo docker run hello-world<br>
OR<br>
sudo apt update;curl -fsSL get.docker.com -o get-docker.sh;sh get-docker.sh;sudo apt install docker-compose;sudo usermod -aG docker $(whoami)<br>
logout<br>
docker run hello-world<br>
<br>



<h1>install docker (https://docs.docker.com/compose/install)</h1>
sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose;sudo chmod +x /usr/local/bin/docker-compose


