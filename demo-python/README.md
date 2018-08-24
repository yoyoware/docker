the following commands will launch a simple python website

docker run -it -p5000:5000 ubuntu bash<br>
apt update<br>
apt-get install -y python python-setuptools python-dev build-essential python-pip python-mysqldb<br>
pip install flask<br>
pip install flask-mysql<br>
cd /opt<br>
cat > /opt/app.py<br>
<br>
import os<br>
from flask import Flask<br>
app = Flask(__name__)

@app.route("/")
def main():
    return "Welcome!"

    @app.route('/how are you')
    def hello():
        return 'I am good, how about you?'

        if __name__ == "__main__":
            app.run()
<br>
<br>
FLASK_APP=app.py flask run --host=0.0.0.0

