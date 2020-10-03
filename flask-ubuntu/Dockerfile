FROM ubuntu 

RUN apt-get update -y 
RUN apt-get install -y python3 python3-pip build-essential
RUN pip3 install flask
RUN mkdir -p /opt/boston_wise

COPY app.py /opt/flask-ubuntu/app.py

ENTRYPOINT FLASK_APP=/opt/flask-ubuntu/app.py FLASK_ENV=development flask run --host=0.0.0.0 
