## Swaggerize the Hyperledger Fabric REST API

This should download the Swagger definition for the [Hyperledger Fabric](https://github.com/hyperledger/fabric/) API, from the current 'master' branch. Copy all of the necessary Swagger dependencies into the current directory, replace the default index.html and launch an http-server which will also open a browser window with the Swagger UI loaded. If you don't see the Fabric API, force a reload of the page to clear any cached content. Specify the swagger definition to load, and hit 'Explore'.

1. Start a peer process. You can use one of the approaches described in the Hyperledger Fabric documentation, [here](http://hyperledger-fabric.readthedocs.io/en/latest/Setup/Network-setup/)

1. The bootstrap.sh script will clone this repository, and launch a Swagger UI for your peer process
   ```
   curl -sS https://raw.githubusercontent.com/christo4ferris/fabric-swagger/master/bootstrap.sh | bash
   ```

For subsequent invocations, execute the `runme.sh` script

```
cd fabric-swagger
./runme.sh
```
