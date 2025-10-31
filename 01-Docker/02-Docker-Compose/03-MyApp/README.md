```
  883  cd 03-MyApp/
  884  ls
  885  cat docker-compose.yaml
  886  docker images
  887  vim docker-compose.yaml
  889  docker-compose up -d
  890  docker ps
  891  docker kill 02-nginx-web1-1
  892  docker-compose up -d
  893  docker kill 03-myapp-db-1
  894  docker-compose ps
  895  docker-compose up -d
  896  docker-compose ps
  897  docker-compose exec proxy ls
  898  docker-compose exec myapp ls
  899  docker-compose exec db ls
  900  docker-compose exec db ps
  901  docker-compose exec db uptime
  902  docker-compose exec db ls -ltr
  903  docker-compose stop
  904  docker-compose ps
  905  docker-compose start proxy
  906  docker-compose ps
  907  docker-compose start db
  908  docker-compose ps
  909  docker-compose stop
  910  docker-compose rm
```
