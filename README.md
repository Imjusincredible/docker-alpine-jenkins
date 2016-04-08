# Jenkins running under Alpine Linux and Oracle JDK 8
[![Docker Repository on Quay.io](https://quay.io/repository/elifarley/alpine-jenkins/status "Docker Repository on Quay.io")](https://quay.io/repository/elifarley/alpine-jenkins) 126.0 MB

``docker pull quay.io/elifarley/alpine-jenkins:latest``

The Jenkins Continuous Integration and Delivery server.

This is a fully functional Jenkins server, based on the Long Term Support release
[http://jenkins-ci.org/](http://jenkins-ci.org/).


<img src="http://jenkins-ci.org/sites/default/files/jenkins_logo.png"/>


# Usage

```
docker run -p 8080:8080 -p 50000:50000 quay.io/elifarley/alpine-jenkins:latest
```

Only a few Alpine packages have been installed, like *curl*, *wget*, *zip* and *bash*.

You can create a derived image and include a few more packages, like this:

```
FROM quay.io/elifarley/alpine-jenkins:latest
MAINTAINER Your Name <your-name@host.com>

USER root

RUN apk --update add --no-cache mercurial git && \
    rm -rf /var/cache/apk/*
    
USER ${user}

```
