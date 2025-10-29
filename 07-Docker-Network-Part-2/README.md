```
 603  docker ps
  604  docker images
  605  docker ps -a
  606  docker images
  607  docker run -d --name ntw-1 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v3
  608  docker ps
  609  docker run -d --name ntw-2 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  610  docker ps
  611  curl 172.17.0.3:80
  612  route -n
  613  ip addr
  614  curl 10.0.8.210
  615  docker ps
  616  docker run -d --name ntw-3 -p 8080:80 amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  617  docker ps
  618  curl 10.0.8.210
  619  curl 10.0.8.210:8080
  620  systemctl  status docker
  621  docker run -d --name ntw-4 -P amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v4
  622  docker run -d --name ntw-5 -P amitvashist7/docker-k8s-ey-wd-27-oct-2025-myapache:v3
  623  docker ps
  624  curl 10.0.8.210:32768
  625  systemctl  status docker
```
