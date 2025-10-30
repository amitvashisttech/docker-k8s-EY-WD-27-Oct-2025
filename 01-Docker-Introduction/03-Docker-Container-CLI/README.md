# Container Commands 

```
   57  docker version
   58  systemctl status docker
   59  docker images
   60  docker container ls
   61  docker container ls -a
   62  docker container ls
   63  docker ps
   64  docker container ls -a
   65  docker ps -a
   66  docker run --name test-av-1 hello-world
   67  docker ps -a
   68  docker run --name test-av-2 hello-world
   69  docker ps -a
   70  docker run -d --name test-av-3 hello-world
   71  docker ps -a
   72  docker run -it --name test-ubuntu-1 ubuntu
   73  docker ps
   74  docker ps -a
   75  docker run -it --name test-ubuntu-2 ubuntu:22.04
   76  docker ps
   77  docker ps -a
   78  ls
   79  docker ps
   80  docker logs test-ubuntu-2
   81  docker logs -f test-ubuntu-2
   82  ls
   83  docker ps
   84  docker attach test-ubuntu-2
   85  ls
   86  docker ps
   87  docker ps -a
   88  docker start test-ubuntu-2
   89  docker ps
   90  ld
   91  ls
   92  docker exec -it test-ubuntu-2 ls
   93  docker exec -it test-ubuntu-2 ls /root
   94  docker exec -it test-ubuntu-2 ls /root/AmitV
   95  docker exec -it test-ubuntu-2 cat /root/AmitV/index.html
```

# Format Commands 
```
 104  docker ps
  105  docker run -itd --name test-ubuntu-3 ubuntu:22.04
  106  docker ps
  107  docker run -itd --name test-ubuntu-4 ubuntu:22.04
  108  docker ps
  109  docker ps -l
  110  docker run -itd --name test-ubuntu-5 ubuntu:22.04
  111  docker ps -l
  112  docker ps
  113  docker ps -q
  114  docker ps -ql
  115  docker inspect $(docker ps -ql)
  116  docker inspect $(docker ps -ql) | wc -l
  117  docker inspect $(docker ps -q) | wc -l
  118  docker inspect $(docker ps -ql)
  119  docker inspect --format '{{.Name}} {{.State.Running}} {{.NetworkSettings.IPAddress}}' $(docker ps -ql)
  120  docker inspect --format '{{.Name}} {{.State.Running}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
  121  docker inspect --format '{{.Name}} {{.State.Running}} {{.NetworkSettings.IPAddress}}' $(docker ps -qa)
  122  docker stop test-ubuntu-4
  123  docker inspect --format '{{.Name}} {{.State.Running}} {{.NetworkSettings.IPAddress}}' $(docker ps -qa)
```

# CleanUp Commands
```
  127  docker ps
  128  docker stop test-ubuntu-5
  129  docker ps
  130  docker kill $(docker ps -q)
  131  docker ps
  132  docker ps -a
  133  docker rm test-ubuntu-5
  134  docker ps -a
  135  docker rm $(docker ps -qa)
  136  docker ps -a
  137  docker ps
  138  docker ps -a
  139  docker images
  140  docker rmi 4f8bb4f91ac0
  141  docker images
  142  docker images -q
  143  docker rmi $(docker images -q)
  144  docker rmi $(docker images -q)  --force
  145  docker images

```
