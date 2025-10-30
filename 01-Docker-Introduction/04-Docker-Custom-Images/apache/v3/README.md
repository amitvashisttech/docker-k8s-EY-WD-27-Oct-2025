```
  319  cd v3/
  320  ls
  323  cat info.html
  324  ls
  325  docker build -t myapache:v3 .
  326  ls
  327  docker build -t myapache:v3 -f MyDockerfile .
  328  docker images
  329  docker run -d --name test-apache-3 myapache:v3
  330  curl 172.17.0.3
  331  curl 172.17.0.4
  332  ls
  333  docker ps
  334  curl 172.17.0.4 -v

```
