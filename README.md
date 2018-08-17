below are some quick (one command line) docker demos<br>
<br>
this site provides FREE docker nodes: www.play-with-docker.com<br>
<br>
nginx on docker<br>
<b>git clone https://github.com/yoyoware/docker;cd docker/demo-nginx;docker-compose up</b><br>
<br>
drupal on docker without persistence<br>
git clone https://github.com/yoyoware/docker;cd docker/demo-drupal;docker-compose up<br>
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
drupal & postgres using overlay<br>
git clone https://github.com/yoyoware/docker;cd docker/demo-drupal-overlay/drupal-node;docker-compose up<br>
<br>
<br>
<br>
<br>
-----------------------------------------------<br>
update git<br>
git config --global user.email "michaelemens@gmail.com";git add -A; git commit -m "comment"; git push origin master<br>





