FROM python:3.8
RUN apt update -y --no-install-recommends && apt install -y --no-install-recommends ffmpeg
RUN mkdir -p /usr/src/api/src
ADD requirements.txt /usr/src/api/
ADD src/server /usr/src/api/src/
WORKDIR /usr/src/api
RUN pip install -r requirements.txt