Docker of graphite + carbon for gatling
========================================

Modifications has been done to https://github.com/nickstenning/docker-graphite so that it can work to receive metrics from gatling.


Instructions:
-------------
1. Do git clone https://github.com/jahangirmohammed/docker-graphite-gatling.git
2. cd docker-graphite-gatling
3. run command - "docker build .". This should create the required image.
4. After the image is created, run the container something like below:
docker run -p 80:80 -p 2003:2003 -p 2004:2004 -p 7002:7002 -d imageName
where imageName is the one created in 3.


For more instructions on ports and data volumes please refer to Nick Stenning's repo - https://github.com/nickstenning/docker-graphite.
