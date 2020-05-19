## devOps -- a collection of personal devOps tools to remember

### jenkins-socat-docker-socket

This `docker-compose` file spins up a `jenkins` and a `socat` command to expose
the docker unix socket to a tcp port, which `jenkins` has access to. The purpose
of this is to run docker commands in a dockerized `jenkins`.

**Notes**

- For the `jenkins` image, at first, I had issues installing it when running the image,
  recommended plugins would fail. With a little googling I found out that there are many
  "official" images for `jenkins`. If you want to know more, please read [this](https://www.jenkins.io/blog/2018/12/10/the-official-Docker-image/)
- The real one is `jenkins/jenkins:lts`. And you can find many flavors like `jenkins/jenkins:jdk11`
  or `jenkins/jenkins:lts-alpine`. Have a look [here](https://hub.docker.com/r/jenkins/jenkins/tags)
