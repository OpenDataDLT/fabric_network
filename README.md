## Build ODPID Blockchain Network

# Step 1 :
***to avoid docker confict with existing containers run these command first***

# stop all running containers
```sh
$ docker stop $(docker ps -aq)
```

# Remove all containers (if needed)
```sh
$ docker rm $(docker ps -aq)
```

# Remove all images (if needed)
```sh
$ docker rmi $(docker images -q)
```


# Step 2 :
***Bootstrap the network and generate the essentials***

```sh
$ ./bootstrap.sh
```

# Step 3 :
***Start Network***

```sh
$ cd odpid-basic-network
$ ./odpid.sh generate
$ ./odpid.sh up -a
```

***Stop Network***

```sh
$ ./odpid-basic-network/odpid.sh down
```


***(Har Preet Singh)***