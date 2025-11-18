FROM ubuntu:latest
RUN apt-get update &&\
apt-get install -y &&\
apt-get install python3 -y &&\
apt-get install python3 python3-pip -y &&\
rm /usr/lib/python*/EXTERNALLY-MANAGED &&\
pip install flask &&\
pip install flask-cors

WORKDIR /app

COPY api.py /app/api.py
CMD ["python3", "api.py"]