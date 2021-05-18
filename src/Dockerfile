FROM ubuntu:bionic

RUN apt-get -y update && apt-get install -y

RUN apt-get -y install libeigen3-dev

COPY main.cpp /home

WORKDIR /home

RUN g++ -I /usr/include/eigen3/ -o eigen-solver main.cpp

CMD [ "./eigen-solver" ]