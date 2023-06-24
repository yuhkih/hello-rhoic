# hello-kubernetes
Nginx test container based on UBI8

## How to build
```
docker build . -t hello-rhoic:latest 
```

## How to use
```
$ docker run --rm --name hello-test -p 80:8080 -d hello-rhoic:latest
$ curl http://localhost 
Hello RHOIC! 
RHOIC is an abbreviation for Red Hat OpenShift on IBM Cloud. It's a managed OpenShift on IBM Cloud.
$ docker stop hello-test
```

