# fabric-samples 

Hyperledger 

$ curl -sSL http://bit.ly/2ysbOFE | sudo bash -s 1.3.0  "install the Fabric Samples and binaries" 

$ cd fabric-samples 

$ export PATH=<path to download location>/bin:$PATH   "to add that to your PATH environment variable so that these can be picked up without fully qualifying the path to each binary." 
  
$ cd first-network   "Let’s open that sub-directory now <fabric-samples/first-network>" 

$ sudo ./byfn.sh generate   "Generate Network Artifacts -- generates all of the certificates and keys for our various network entities, the genesis block used to bootstrap the ordering service, and a collection of configuration transactions required to configure a Channel" 

$ sudo ./byfn.sh up   "Bring Up the Network -- compile Golang chaincode images and spin up the corresponding containers" 

$ sudo ./byfn.sh down  "Bring Down the Network --bring it all down so we can explore the network setup one step at a time. The following will kill your containers, remove the crypto material and four artifacts, and delete the chaincode images from your Docker Registry" 

