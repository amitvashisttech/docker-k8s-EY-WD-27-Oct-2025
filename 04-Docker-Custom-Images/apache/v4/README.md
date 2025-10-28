```
  340  cd v4/
  342  cat MyDockerfile
  344  cat info.html
  345  ls
  346  docker build -t myapache:v4 -f MyDockerfile .
  347  cat MyDockerfile
  348  ls
  349  docker run -d --name test-apache-4 myapache:v4
  350  docker ps
  351  curl 172.17.0.5:80
  352  curl 172.17.0.5:8080
  353  curl 172.17.0.5:81

```
