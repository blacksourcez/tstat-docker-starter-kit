# Tstat in docker

Tstat in container, see more on [Docker Hub](https://hub.docker.com/r/ayuthmang/tstat).

## Build docker file to docker image

```bash
docker build 3/ubuntu/
```

## Using Tstat on Container

```bash
$ docker run --name=bs-tstat --rm --net=host -it -v /root/tstat-logs:/root/tstat-logs blacksource/tstat tstat -l -i <your interface name> -s /root/tstat-logs
```

## Special Thanks

Thanks for https://hub.docker.com/r/andreyferriyan/tstat/ for make run command fullfilled.

## License

Tstat is provided under the GPL software license and made available for free for personal and research usage. If you plan to use it for commercial usage, [you should go to their homepage](http://tstat.polito.it/software.php). 
