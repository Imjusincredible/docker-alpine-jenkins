# Alpine-based Jenkins Docker image
[![Docker Repository on Quay.io](https://quay.io/repository/elifarley/alpine-jenkins/status "Docker Repository on Quay.io")](https://quay.io/repository/elifarley/alpine-jenkins)

``docker pull quay.io/elifarley/alpine-jenkins:latest``

The Jenkins Continuous Integration and Delivery server.

This is a fully functional Jenkins server, based on the Long Term Support release
[http://jenkins-ci.org/](http://jenkins-ci.org/).


<img src="http://jenkins-ci.org/sites/default/files/jenkins_logo.png"/>


# Usage

```
docker run -p 8080:8080 -p 50000:50000 quay.io/elifarley/alpine-jenkins:latest
```

