below are some quick (one command line) docker demos<br>
<br>
if you don't have an OS running docker, this site provides FREE docker nodes: www.play-with-docker.com<br>
<br>
<h1>nginx</h1>(with volume persistence)
cd;git clone https://github.com/yoyoware/docker;cd docker/demo-nginx-with-volume;docker-compose up<br>
<br>
<h1>drupal (with volume persistence)</h1>cd;git clone https://github.com/yoyoware/docker;cd docker/demo-drupal-with-volume;docker-compose up<br>
configuration: language = english, profile = standard, database = postgres, database name = postgres, database username = postgres, password = mypassword, advanced options host = postgres, site configure page: enter all required fields to your choice<br>
<br>
<h1>jenkins (with volume persistence)</h1>
cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-jenkins-with-volume;mkdir my-jenkins-data;chmod 777 my-jenkins-data;docker-compose up<br>
<br>
<br>
<br>
<br>
-----------------------------------------------<br>
update git<br>
<b>cd; rm -rf ./docker/demo-jenkins-with-volume/my-jenkins-data;cd ./docker;git config --global user.email "michaelemens@gmail.com";git pull;git add -A; git commit -m "comment"; git push origin master</b><br>




