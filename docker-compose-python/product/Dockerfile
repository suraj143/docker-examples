FROM python:3-onbuild
MAINTAINER Raj Gajjelli "raj.gajjelli@gmail.com"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
COPY . /usr/src/app
WORKDIR /usr/src/app
RUN pip install -r requirements.txt
CMD ["python", "api.py"]