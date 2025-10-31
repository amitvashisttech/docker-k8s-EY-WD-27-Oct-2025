# Docker Images Tagging - Push & Pull 

```
 452  cd 05-Docker-Image-Tags/
  453  ls
  454  docker images
  455  docker login -u amitvashist7
  456  docker push myapache:v1
  457  docker tag 9c758c066977 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v1
  458  docker images
  459  docker tag 945dc56c674e amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v2
  460  docker tag a55571b9e090 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v3
  461  docker tag ff19bf2bf21e amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  462  docker images
  463  docker push amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v1
  464  docker push amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v2
  465  docker push amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v3
  466  docker push amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  467  ls
  468  docker logout
  469  ls
  470  docker images
  471  docker kill $(docker ps -q)
  472  docker rm $(docker ps -qa)
  473  docker rmi $(docker images -q) --force
  474  docker images
  475  docker ps -a
  476  docker run -d --name apache-1 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v1
  477  docker ps
  478  docker run -d --name apache-2 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v2
  479  docker run -d --name apache-3 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v3
  480  docker run -d --name apache-4 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  481  ls
  482  docker ps
  483  curl 172.17.0.2
  484  curl 172.17.0.3
  485  curl 172.17.0.4
  486  curl 172.17.0.5
```
