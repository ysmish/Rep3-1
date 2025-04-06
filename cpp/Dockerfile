FROM gcc:latest

RUN apt-get update && apt-get install -y cmake

COPY . /user/src/mytest
WORKDIR /user/src/mytest

RUN mkdir build
WORKDIR /user/src/mytest/build

RUN cmake .. && make

CMD [ "./runTests" ]