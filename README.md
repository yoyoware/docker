below are some quick (one command line) docker demos<br>
<br>
this site provides FREE docker nodes: www.play-with-docker.com<br>
<br>
nginx (with volume persistence)<br>
<b>cd;git clone https://github.com/yoyoware/docker;cd docker/demo-nginx-with-volume;docker-compose up</b><br>
<br>
drupal on docker (with volume persistence)<br>
<b>cd;git clone https://github.com/yoyoware/docker;cd docker/demo-drupal-with-volume;docker-compose up</b><br>
configuration:<br>
language = english<br>
profile = standard<br>
database = postgres<br>
database name = postgres<br>
database username = postgres<br>
password = mypassword<br>
advanced options host = postgres<br>
site configure page: enter all required fields to your choice<br>
<br>
jenkins (with volume persistence)<br>
<b>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-jenkins-with-volume;mkdir my-jenkins-data;chmod 777 my-jenkins-data;docker-compose up</b><br>
<br>
<br>
<br>
<br>
-----------------------------------------------<br>
update git<br>
<b>cd; rm -rf ./docker/demo-jenkins-with-volume/my-jenkins-data;cd ./docker;git config --global user.email "michaelemens@gmail.com";git pull;git add -A; git commit -m "comment"; git push origin master</b><br>




