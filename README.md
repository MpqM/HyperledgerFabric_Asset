# HyperledgerFabric_v1.x-SimpleAsset
<!-- 1 -->
#### ⚫ About Project
##### build HyperLedgerFabric application 
##### with Node, Express, Javascript, HTML
##### Learn how to build a Basic full-stack HyperlegderFabric app through clonecoding with React, Node, Express, MongoDB Atlas, and TypeScript
* * *
<!-- 2 -->
#### ⚫ Built with
<img alt="Html" src ="https://img.shields.io/badge/HTML5-E34F26.svg?&style=for-the-badge&logo=HTML5&logoColor=white"/> <img alt="JavaScript" src ="https://img.shields.io/badge/JavaScriipt-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=white"/> <img alt="typescript" src ="https://img.shields.io/badge/hyperledger-3178C6.svg?&style=for-the-badge&logo=hyperledger&logoColor=white"/> <img alt="express" src ="https://img.shields.io/badge/express-339933.svg?&style=for-the-badge&logo=express&logoColor=white"/> <img alt="nodedotjs" src ="https://img.shields.io/badge/nodejs-339933.svg?&style=for-the-badge&logo=nodedotjs&logoColor=white"/> 
* * *
<!-- 3 -->
#### ⚫ Getting Strated
* ##### Prerequisites
   * ##### npm, node, MongoDB Atlas account
* ##### installation
   * ##### set up MongoDB Atlas and connect
   * ##### Change the MONGO_CONNECTION_STRING value in the server/.env file with yours
   * ##### git clone https://github.com/MpqM/MERN_Note.git
   * ##### cd server -> npm install -> npm start
   * ##### cd client -> npm install -> npm start
* * *
<!-- 4 -->
#### ⚫ description
* ##### I studied by adding annotations and testing api with postman, not just copying and pasting code.
* ##### I practiced the composition of the readme file and I think it was organized well as a result

* * *
<!-- 5 -->
#### ⚫ Usage

* * *
<!-- 6 -->
#### ⚫ Roadmap & Realization

* * *
<!-- 7 -->
#### ⚫ Writer
* ##### okqkrwhdtjd@gmail.com
* ##### <a href = "https://github.com/MpqM"><img alt="GitHub" src ="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/></a> <a href = "https://MpqM.tistory.com/"> <img alt="Tistory" src ="https://img.shields.io/badge/Tistory-white.svg?&style=for-the-badge"/></a>
* * *
<!-- 8 -->
#### ⚫ Contributing
* ##### Fork the Project https://github.com/MpqM/HyperledgerFabric_v1.x-SimpleAsset
* ##### Create your Feature Branch (git checkout -b feature/AmazingFeature)
* ##### Commit your Changes (git commit -m 'Add some AmazingFeature')
* ##### Push to the Branch (git push origin feature/AmazingFeature)
* ##### Open a Pull Request
* * *
<!-- 9 -->
#### ⚫ Acknowledgments & License
* 
* * * *



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

**Set-Up**
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
