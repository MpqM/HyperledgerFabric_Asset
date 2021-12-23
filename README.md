**Development Enviorment Setting**

* basic
  * ubuntu 18.04.5
  * virtualmachine

* curl
  * sudo apt-get update
  * sudo apt-get install curl
  * if err-> sudo reboot -> try again
  * curl --version
  
* docker
  * sudo apt install docker.io docker-compose -y
  * sudo apt-get install software-properties-common
  * sudo usermod -aG docker $USER
  * echo $USER
  * reboot
  * docker version
  * docker-compose version

* node.js
  * sudo apt-get install build-essential libssl-dev -y
  * curl -OL https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
  * bash install.sh
  * source .profile
  * nvm install v8
  * node -v
  * npm -v
  
* go
  * curl -OL https://golang.org/dl/go1.12.17.linux-amd64.tar.gz
  * tar -xvf go1.12.17.linux-amd64.tar.gz
  * sudo mv go /usr/local
  * gedit .profile
  * add two lines in last
    * export GOPATH=~/go
    * export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin:~/fabric-samples/bin
  * source .profile
  * echo $PATH
  * go version
  
* python, git, vsc
  * sudo apt install -y python
  * sudo apt install -y git
  * install vsc, go, docker extension

* hyperledgerfabric
  * curl -sSL http://bit.ly/2ysbOFE | bash -s -- 1.4.12 1.4.9 0.4.22

**set-up**
* clone code

* network
 * spec : 3 org(each have 1 peer) 1 ca 1 order
 * cd network
 * ./teardown.sh
 * ./generate.sh
 * ./start.sh 

* chaincode install, instsantiate, test
 * go build 
 * if err try underlines
 * go get -u "github.com/hyperledger/fabric/chaincode/shim" 
 * cd $GOPATH cd src/github.com/hyperledger/fabric
 * git checkout tags/v1.4.10
 * ./cc.sh
 * ./testasset.sh

* application
 * cd application
 * npm install
 * node enrollAdmin.js
 * node registerUser.js
 * node server.js
 * connect to localhost:8080
 * check asset localhost:5984/_utils

**Running Screen**
