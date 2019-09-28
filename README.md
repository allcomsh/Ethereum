# Ethereum
All about ethereum regarding DAPP development
https://github.com/ethereum/go-ethereum/wiki/Building-Ethereum

#Centos
https://golang.org/dl/
modify ~/.bash_profile add go/bin to PATH

#Windows:
 https://github.com/ethereum/go-ethereum/wiki/Installation-instructions-for-Windows
 go get -u -v golang.org/x/net/context
 # if failed, do this first:
 $mkdir -p $GOPATH/src/golang.org/x/
 $cd $GOPATH/src/golang.org/x/ 
 $git clone https://github.com/golang/net.git net 
 $go install net
https://www.cnblogs.com/weifeng1463/p/7488862.html

 go install -v ./cmd/...
 
# Books
https://github.com/ethereumbook/ethereumbook

# Download
 https://geth.ethereum.org/downloads/
 need genisys file devnet.json and static-nodes.json
1.  geth --datadir node1 init devnet.json
2.  geth --datadir node1 --syncmode full --port 30303 --rpc --rpcaddr "0.0.0.0" --rpcport 8545 --rpcapi "personal,db,eth,net,web3,txpool,miner" --bootnodes "enode://11e1d914c7d4b09f5cbf6ff238ee9fede90fc8cb60484856848421971203b58484023b44771161dc229447b398fbaf4b122611d282bda54555c3089cb3c294b6@118.190.79.30:30307" --networkid 1515 --gasprice 1  --lightserv 30 --rpccorsdomain "*" console

geth在KVM的centos虚拟机中运行时导致宿主机和虚拟机的CPU占用高

# get release version
git clone https://github.com/ethereum/go-ethereum.git go-ethereum-1.8

git branch -a

git checkout remotes/origin/release/1.8
