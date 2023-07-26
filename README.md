# HyperledgerFabric_v1.x-SimpleAsset
#### ⚪ About Project
* ##### 단순한 자산 데이터에 대한 CRUD 기능을 가진 체인코드를 NodeJs Express 모듈 기반 RESTAPI를 통해 체인 코드를 테스트하는 웹 어플리케이션
* ##### Node, Express, Javascript, HTML을 사용해 HyperLedgerFabric 웹 응용 프로그램 구축
* * *
#### ⚪ Usage
![image](https://github.com/MpqM/HyperledgerFabric_v1.x-SimpleAsset/assets/79093184/9bf5a1db-9a72-4054-9b72-1f592cc222b4)
* * *
#### ⚪ Built with
* ##### Frontend
<img alt="Html" src ="https://img.shields.io/badge/HTML5-E34F26.svg?&style=for-the-badge&logo=HTML5&logoColor=white"/> <img alt="JavaScript" src ="https://img.shields.io/badge/JavaScriipt-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=white"/>
* ##### Backend
<img alt="express" src ="https://img.shields.io/badge/express-339933.svg?&style=for-the-badge&logo=express&logoColor=white"/> <img alt="nodedotjs" src ="https://img.shields.io/badge/nodejs-339933.svg?&style=for-the-badge&logo=nodedotjs&logoColor=white"/> 
* ##### Private Blockchain
<img alt="typescript" src ="https://img.shields.io/badge/hyperledger-3178C6.svg?&style=for-the-badge&logo=hyperledger&logoColor=white"/>


* * *

#### ⚪ Getting Strated
* ##### Prerequisites: Ubuntu 18.04.5, virtualmachine
* ##### Installation
```bash
# curl
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
* ##### Execution
```bash
clone repo
# network
spec : 3 org(each have 1 peer) 1 ca(artificial) 1 order
cd network
./teardown.sh
./generate.sh
./start.sh
# chaincode install, instsantiate, test
go build
/* if err try underlines
   go get -u "github.com/hyperledger/fabric/chaincode/shim"
*/
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
* * *
#### ⚪ Description
* ##### 하이퍼레저 패브릭 네트워크 구조를 로컬호스트에서 구축
* ##### GO언어 기반 CRUD기능을 가진 체인코드를 작성
* ##### NodeJs의 express모듈을 통해 RestAPI를 구축하고 HTML을 통해 홈페이지를 만들어 CRUD 기능 테스트 수행
* * *
#### ⚪ Roadmap & Realization & Study
* ##### 하이퍼레저 패브릭 버전1.x는 현재 오래되서 v2.x로 업데이트 추천
* ##### 하이퍼레저 패브릭 v2.x 공부할예정
* * *
#### ⚪ Writer
* ##### okqkrwhdtjd@gmail.com
* ##### <a href = "https://github.com/MpqM"><img alt="GitHub" src ="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/></a> <a href = "https://MpqM.tistory.com/"> <img alt="Tistory" src ="https://img.shields.io/badge/Tistory-white.svg?&style=for-the-badge"/></a>
* * *
#### ⚪ Contributing
* ##### Fork the Project https://github.com/MpqM/HyperledgerFabric_v1.x-SimpleAsset
* ##### Create your Feature Branch (git checkout -b feature/AmazingFeature)
* ##### Commit your Changes (git commit -m 'Add some AmazingFeature')
* ##### Push to the Branch (git push origin feature/AmazingFeature)
* ##### Open a Pull Request
* * *
#### ⚫ Acknowledgments & License
* ##### @[Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
* ##### https://hyperledger-fabric.readthedocs.io/ko/latest
