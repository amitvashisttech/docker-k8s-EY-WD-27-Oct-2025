```
 275  cat Dockerfile
  276  docker run -it --name test-web ubuntu:noble
  277  ls
  278  cat Dockerfile
  279  ls
  280  docker build -t myapache:v1 .
  281  docker images
  282  docker run -d --name test-apache-1 myapache:v1
  283  docker ps
  284  docker inspect test-apache-1
  285  curl 172.17.0.2
```
