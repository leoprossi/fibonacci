# Fibonacci [![Build Status](https://travis-ci.org/leoprossi/fibonacci.svg?branch=master)](https://travis-ci.org/leoprossi/fibonacci)

## Intro
A simple set of apps for me to train docker-compose and test some tools like travis and Amazon EBS. It basically returns the due number from the fibonacci's sequence given one index. The application code itself is not mine, it's got a few bugs and I'm going to work better on it later, as soon as I get everything to work propperly with the containers.

## Running locally
Assuming you have `docker-compose` installed on your machine, you can just go for `docker-compose up` from the root of the project and everything is gointg to be up and running in a few seconds, including a persistent instance of a Postgres database and the Redis server used by the application.
There's a volume mapped for the `client` app's source code ensuring that the hot reload works from inside the container, so just turn everything up once and the container will be able to reload the app as you edit the files.


## Production
Still working on this part.