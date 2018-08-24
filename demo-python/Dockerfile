FROM ubuntu

RUN apt update
RUN apt-get install -y python
RUN apt-get install -y python-pip
RUN pip install flask

EXPOSE 5000

COPY app.py /opt/app.py

ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0

