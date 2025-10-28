```
  302  cd v2/
  303  ls
  304  vim Dockerfile
  305  ls
  306  vim info.html
  307  ls
  308  docker build -t myapache:v2 .
  309  docker images
  310  docker run -d --name test-apache-2 myapache:v2
  311  docker ps
  312  curl 172.17.0.2
  313  curl 172.17.0.3

```
