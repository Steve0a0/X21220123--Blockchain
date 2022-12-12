## Build an Image ##

```docker build --tag nci02 .```


## Run an image ##

```docker run --name ncilab02 -p 8090:8080 nci02```

## This transfers ETH: ##

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\":\"destination address\", \"amount\":\"0.05\"}' http://localhost:8090/eth```



## This transfers token: ##

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"destination address\"}' http://localhost:8090/token```

