# set the base image to Ubuntu
FROM ubuntu

# File Author / Maintainer
MAINTAINER Eder Roger Souza

# update the repository and install Redis Server
RUN apt-get update && \
    apt-get install -y --no-install-recommends redis-server && \
    rm -rf /var/lib/apt/lists/*

# Expose Redis port 6379
EXPOSE 6379

# Run Redis server
ENTRYPOINT ["/usr/bin/redis-server"]
