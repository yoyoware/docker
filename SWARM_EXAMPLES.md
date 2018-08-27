below are some docker swarm commands<br>
<br>
if you don't have an OS running docker, this site provides FREE docker nodes: www.play-with-docker.com<br>
<br>
<b>#initialize this node as swarm MANAGER</b><br>
docker swarm init --advertise-addr 192.168.0.46

<b>#start other nodes as WORKER</b><br>
copy/paste swarm token command line to each worker node in swarm

<b>#list all nodes is swarm</b><br>
docker node ls

<b>#start nginx in a single container in ONE of the swarm nodes</b><br>
docker service create --name "rule-the-world" -p 80:80 nginx

<b>#start nginx in a single container in ALL of the swarm nodes</b><br>
docker service create --name "rule-the-world" -p 80:80 --mode global nginx

<b>#start nginx in a x replica containers of the swarm nodes</b><br>
docker service create --name "rule-the-world" -p 80:80 --replicas 2 nginx

<b>#start alpine container in one of the swarm nodes</b><br>
docker service create --name "pingnode1" alpine ping 192.168.0.18<br>
docker service ls<br>
docker service ps pingnode1<br>
on target node run: docker ps<br>
on target node run: docker logs -f <container id><br>

<b>#start jenkins in a single container in ONE of the swarm nodes</b><br>
docker service create --name "iam_jenkins" --replicas 2 -p 8080:8080 jenkins
docker service ls<br>
docker service ps iam_jenkins<br>
on target node run: docker ps<br>
on target node run: docker logs -f <container id><br>

<b>#increase the number of replicas for a given service</b><br>
docker service scale rule-the-world=5<br>
docker service scale rule-the-world=10<br>
docker service scale rule-the-world=20<br>
docker service scale rule-the-world=100<br>
docker service scale rule-the-world=1000<br>

<b>#list the services running in the swarm along with replicas</b><br>
docker service ls

<b>#list the named service along with the nodes it is running on</b><br>
docker service ps rule-the-world

<b>#list the containers running</b><br>
docker ps

<b>#remove service</b><br>
docker service rm rule-the-world

<b>#change a node avaiability to not active - preventing services from being run there</b><br>
docker node update --availability drain node1;docker node ls

<b>#change a node avaiability to active - allowing services to run there</b><br>
docker node update --availability active node1;docker node ls




