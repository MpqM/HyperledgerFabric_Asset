# HyperledgerFabric-SimpleAsset
#### ⚪ About Project
* NodeJS express, Javascript, HTML을 사용해 CRUD기능을 가진 HyperLedgerFabric DApp 구축
* 단순한 asset 데이터에 대한 CRUD 기능을 가진 체인코드를 NodeJS express 기반 RESTAPI를 통해 테스트
* HyperledgerFabric version ^1.x 사용, 3 org(each have 1 peer) 1 ca(cryptogen) 1 order

- - -

#### ⚪ Running Screen || Video
<p align ="center">
   <img src="https://github.com/MpqM/HyperledgerFabric_v1.x-SimpleAsset/assets/79093184/9bf5a1db-9a72-4054-9b72-1f592cc222b4.png"/>
</p>

- - -

#### ⚪ Built with
<p align ="center">
   <img alt="Html" src ="https://img.shields.io/badge/HTML5-E34F26.svg?&style=for-the-badge&logo=HTML5&logoColor=white"/> <img alt="JavaScript" src ="https://img.shields.io/badge/JavaScriipt-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=white"/> <img alt="express" src ="https://img.shields.io/badge/express-339933.svg?&style=for-the-badge&logo=express&logoColor=white"/> <img alt="nodedotjs" src ="https://img.shields.io/badge/nodejs-339933.svg?&style=for-the-badge&logo=nodedotjs&logoColor=white"/> <img alt="typescript" src ="https://img.shields.io/badge/hyperledger-3178C6.svg?&style=for-the-badge&logo=hyperledger&logoColor=white"/>
</p>

- - -

#### ⚪ Getting Started
```bash
# prerequisites
# curl
Ubuntu 18.04.5, virtualmachine
sudo apt-get update
sudo apt-get install curl
if err-> sudo reboot -> try again
curl --version
# docker
sudo apt install docker.io docker-compose -y
sudo apt-get install software-properties-common
sudo usermod -aG docker $USER
echo $USER
reboot
docker version
docker-compose version
# NodeJs
sudo apt-get install build-essential libssl-dev -y
curl -OL https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
bash install.sh
source .profile
nvm install v8
node -v
npm -v
# go
curl -OL https://golang.org/dl/go1.12.17.linux-amd64.tar.gz
tar -xvf go1.12.17.linux-amd64.tar.gz
sudo mv go /usr/local
gedit .profile
# add under two lines in last
export GOPATH=~/go
export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin:~/fabric-samples/bin
source .profile
echo $PATH
go version
# python, git, vsc
sudo apt install -y python
sudo apt install -y git
install vsc, go, docker extension
# hyperledgerfabric
curl -sSL http://bit.ly/2ysbOFE | bash -s -- 1.4.12 1.4.9 0.4.22
```
```bash
# execution
clone repo
# network
spec : 3 org(each have 1 peer) 1 ca(artificial) 1 order
cd network
./teardown.sh
./generate.sh
./start.sh
# chaincode install, instsantiate, test
go build
# if err try underlines
# go get -u "github.com/hyperledger/fabric/chaincode/shim"
 cd $GOPATH cd src/github.com/hyperledger/fabric
git checkout tags/v1.4.10
./cc.sh
./testasset.sh
# application
cd application
npm install
node enrollAdmin.js
node registerUser.js
node server.js
connect to localhost:8080
check asset localhost:5984/_utils
```

- - -

#### ⚪ Description
* ##### 하이퍼레저 패브릭 네트워크를 로컬호스트 환경에서 구축
* ##### GO언어 기반 트랜잭션에 대한 CRUD기능을 가진 체인코드 작성
* ##### NodeJs의 express모듈을 통해 RestAPI를 구축하고 HTML을 통해 홈페이지를 만들어 CRUD 기능 테스트 수행

- - -

#### ⚪ Writer
<p align ="center">
  <img src ="https://img.shields.io/badge/gmail-EA4335.svg?&style=for-the-badge&logo=gmail&logoColor=white"/></a> <a href = "https://github.com/MpqM"><img src ="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/></a> <a href = "https://MpqM.tistory.com/"> <img src ="https://img.shields.io/badge/tistory-000000.svg?&style=for-the-badge&logo=Tistory&logoColor=white"/></a>
</p>

- - -
