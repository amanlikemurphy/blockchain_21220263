## Build an Image ##

```docker build --tag amanlikemurphy/murphy-x21220263 .```


## Run an image ##

```docker run -p 8090:8080 --name nci05 -d amanlikemurphy/murphy-x21220263```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x7aC3D1dEd92DB2E5DfAE74cF52d4Da9f92aaed76", "amount":"0.05"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x7aC3D1dEd92DB2E5DfAE74cF52d4Da9f92aaed76"}' http://localhost:8090/token```

