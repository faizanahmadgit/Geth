1:  geth --datadir mychain1 account new 
2:  geth --datadir ./mychan1 init ../genesis.json
3:  geth --datadir ./mychan2 init ../genesis.json
4:  bootnode -genkey boot.key
5:  bootnode -nodekey boot.key
6: bootnode -nodekey "./boot.key" -verbosity 7 -addr "127.0.0.1:30301"
7: For Node 1: geth --networkid 17 --datadir "./mychain1" --boo
tnodes enode://73465801a206aea7938d8a23de0abdc47297b467c703bae1146d9bd00f56559ff74499f74798d271adf40fb42814b44d8ba83af651589ac7e6f34786b2c9a1bd@127.0.0.1:30301 -
-port 30303 --ipcdisable --syncmode full —http --allow-insecure-unlock --rpccors
domain "*" —http.port 8545 --unlock 64dd2c86ea06908cafe694d44897e1df70e58cb2 --pa
ssword password.txt --mine console

8: For Node 2 :     geth --networkid 17 --datadir "./mychain2" --bootnodes enode://73465801a206aea7938d8a23de0abdc47297b467c703bae1146d9bd00f56559ff74499f74798d271adf40fb42814b44d8ba83af651589ac7e6f34786b2c9a1bd@127.0.0.1:30301 --port 30304 --ipcdisable --syncmode full --allow-insecure-unlock --unlock 8d4b93f0ad2c17af5857bb1d913eb47d1bd3a031 --password password.txt  console    
