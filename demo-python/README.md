the following commands will launch a simple python website

docker run -it -p5000:5000 ubuntu bash
apt update
apt-get install -y python python-setuptools python-dev build-essential python-pip python-mysqldb
pip install flask
pip install flask-mysql
cd /opt
cat > /opt/app.py
import os
from flask import Flask
app = Flask(__name__)

@app.route("/")
def main():
    return "Welcome!"

    @app.route('/how are you')
    def hello():
        return 'I am good, how about you?'

        if __name__ == "__main__":
            app.run()

FLASK_APP=app.py flask run --host=0.0.0.0

