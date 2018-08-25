<b>#initialize this node as swarm MASTER</b><br>
docker swarm init --advertise-addr 192.168.0.46

<b>#start other nodes as WORKER</b><br>
copy/paste swarm token command line to each worker node in swarm

<b>#list all nodes is swarm</b><br>
docker node ls

<b>#start nginx in the swarm</b><br>
docker service create --name "rule-the-world" -p 80:80 nginx

<b>#list the services running in the swarm along with replicas</b><br>
docker service ls

<b>#list the containers running</b><br>
docker ps

<b>#list the saervices running along with the nodes they are running on</b><br>
docker service ps rule-the-world

<b>#this line will deploy the image to all available nodes in swarm</b><br>
docker service create --name "rule-the-world" -p 80:80 --mode global nginx


