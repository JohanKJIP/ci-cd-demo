FROM ubuntu:latest
RUN apt update
RUN apt-get update -y
RUN apt-get install -y python3-pip python-dev build-essential
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt
RUN pytest ./tests
ENTRYPOINT ["python3"]
CMD ["app.py"]
