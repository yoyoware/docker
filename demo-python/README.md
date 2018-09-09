www.play-with-docker.com<br>
<h1>docker run</h1>
docker run -it -p 5000:5000 ubuntu bash<br>
apt update<br>
apt-get install -y python python-setuptools python-dev build-essential python-pip python-mysqldb<br>
pip install flask<br>
pip install flask-mysql<br>
cd /opt<br>
cat > /opt/app.py<br>
<br>
<b>
import os<br>
from flask import Flask<br>
app = Flask(__name__)<br>
<br>
@app.route("/")<br>
def main():<br>
    return "Welcome!"<br>
<br>
    @app.route('/how are you')<br>
    def hello():<br>
        return 'I am good, how about you?'<br>
<br>
        if __name__ == "__main__":<br>
            app.run()<br>
</b>
<br>
<br>
FLASK_APP=/opt/app.py flask run --host=0.0.0.0

docker build -t mypython:latest .
docker run mypython -p5000:5000





<h1>docker-compose with bash</h1>
cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-jenkins;sudo docker-compose up -d<br>
docker exec -it demo bash


the following commands will launch a simple python website

