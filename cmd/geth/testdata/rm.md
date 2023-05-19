
./octa-geth --datadir /home/panda/.otca --networkid 800001 --port 30312 --http --http.port 9722 --authrpc.port 8782 --http.api personal,eth,net,web3,admin,txpool,debug --cache=8000 --maxpeers 100 --syncmode full --password /home/panda/.elh/.elh-pw --nat any --allow-insecure-unlock --snapshot=false  --ipcpath "~/.octa/geth.ipc" --miner.gasprice "1000000000" --miner.gastarget "50000000" --miner.gaslimit "50000000"

./otca-geth --datadir /home/panda/.otca account new

0xcC026343D617b6780C7D75495940E67efa763285

./otca-geth --datadir /home/panda/.otca --networkid 61803 --port 30311 --http --http.port 9721 --http.api personal,eth,net,web3,admin,txpool,debug --cache=8000 --maxpeers 100 --syncmode full --password /home/panda/.elh/.elh-pw --nat any --allow-insecure-unlock --snapshot=false  --ipcpath "~/.etica/geth.ipc" --miner.gasprice "1000000000" --miner.gastarget "50000000" --miner.gaslimit "50000000" --bootnodes "enode://b0e97d2f1a37b2035a34b97f32fb31ddd93ae822b603c56b7f17cfb189631ea2ef17bfbed904f8bc564765634f2d9db0a128835178c8af9f1dde68ee6b5e2bf7@167.172.47.195:30303" --mine --miner.etherbase 0xcC026343D617b6780C7D75495940E67efa763285 --unlock 0xcC026343D617b6780C7D75495940E67efa763285

./otca-geth attach /home/panda/.otca/geth.ipc

admin.addPeer("enode://...")

admin.peers <<< to show peers list


./build/bin/geth --networkid 800001 --mine --miner.threads=2 --nat extip:127.0.0.1 --miner.gasprice "1000000000" --miner.gastarget "50000000" --miner.gaslimit "50000000" --datadir "./eticanode1" --http --http.addr "localhost" --authrpc.port 8782 --http.port "8545" --port "30303" --allow-insecure-unlock --http.corsdomain "*" --nat "any"  --rpc.allow-unprotected-txs  --http.api eth,web3,personal,net --rpcvhosts=* --ipcpath "~/.ethereum/geth.ipc" --bootnodes "enode://b0e97d2f1a37b2035a34b97f32fb31ddd93ae822b603c56b7f17cfb189631ea2ef17bfbed904f8bc564765634f2d9db0a128835178c8af9f1dde68ee6b5e2bf7@167.172.47.195:30303"
