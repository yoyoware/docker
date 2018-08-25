#initialize this node as swarm MASTER
docker swarm init --advertise-addr 192.168.0.46

#start other nodes as WORKER
copy/paste swarm token command line to each worker node in swarm

#list all nodes is swarm
docker node ls

#start nginx in the swarm
docker service create --name "rule-the-world" -p 80:80 nginx

#list the services running in the swarm along with replicas
docker service ls

#list the containers running
docker ps

#list the saervices running along with the nodes they are running on
docker service ps rule-the-world

#this line will deploy the image to all available nodes in swarm
docker service create --name "rule-the-world" -p 80:80 --mode global nginx


