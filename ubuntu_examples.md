https://djangostars.com/blog/what-is-docker-and-how-to-use-it-with-python/

<h1>ubuntu ls</h1>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-ubuntu-ls;sudo docker-compose up<br>
<h1>ubuntu +echo hello world</h1>docker run ubuntu /bin/echo 'Hello world'  
<h1>ubuntu +interactive terminal bash</h1>docker run -i -t --rm ubuntu /bin/bash    
<h1>container running after the end of the session</h1>docker run --name daemon -d ubuntu /bin/sh -c "while true; do echo hello world; sleep 1; done"  
