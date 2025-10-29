## Static Volumes 

```
  640  docker ps
  641  docker kill $(docker ps -q)
  642  docker rm $(docker ps -q)
  643  docker rm $(docker ps -qa)
  644  docker volume ls
  645  docker volume create myvol1
  646  docker volume ls
  647  docker volume inspect myvol1
  648  ls -ltr /var/lib/docker/volumes/myvol1/_data
  649  docker run -it stg-1 -v myvol1:/myapp ubuntu
  650  docker run -it --name stg-1 -v myvol1:/myapp ubuntu
  651  ls
  652  ls -ltr /var/lib/docker/volumes/myvol1/_data
  653  ls -ltr /var/lib/docker/volumes/myvol1/_data/amit/
  654  cat  /var/lib/docker/volumes/myvol1/_data/amit/index.html
  655  ls
  656  docker ps
  657  docker inspect  stg-1
  658  ls
  659  docker run -it --name stg-2 -v myvol1:/var/www/html ubuntu
  660  docker ps
  661  docker run -it --name stg-3 -v myvol1:/abc:ro ubuntu
```


## Dynamic Volume
```
681  docker exec -it stg-2 ls -ltr /var/www/html/
  682  docker exec -it stg-2 cat /var/www/html/amit/index.html
  683  cd
  684  ls
  685  docker run -it --name stg-dynamic-1 -v /myvol-a ubuntu
  686  docker ps
  687  docker inspect stg-dynamic-1
  688  docker volume ls
  689  cat /var/lib/docker/volumes/83daec1a38ac20c6de4f4a368df03ca5f4787924f030bd12c2dc4e256b1c1243/_data/abc.txt
  690  docker run -itd --name stg-dynamic-2 -v /myvol-a -v /myvol-b -v /myvol-c -v /myvol-123 ubuntu
  691  docker ps
  692  docker inspect stg-dynamic-2
  693  docker volume ls
  694  ls
  695  docker ps
  696  docker kill $(docker ps -q)
  697  docker rm $(docker ps -aq)
  698  docker ps
  699  docker ps -a
  700  docker volume ls
  701  cat /var/lib/docker/volumes/myvol1/_data/amit/index.html
  702  cat /var/lib/docker/volumes/83daec1a38ac20c6de4f4a368df03ca5f4787924f030bd12c2dc4e256b1c1243/_data/abc.txt
  703  ls
  704  docker volume ls -q
  705  docker volume rm $(docker volume ls -q)
  706  docker volume ls
```
