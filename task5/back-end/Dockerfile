FROM ubuntu:latest
RUN apt-get update \
	&& apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask
RUN pip3 install flask-cors
WORKDIR /app
COPY . .
CMD [ "python3", "api.py" ]
