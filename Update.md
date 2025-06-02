## Update 3 ; 

```bash
screen -r aztec
```

- CTRL + C - Stop your Node

#### Delete Your Database 

```bash
rm -rf ~/.aztec/alpha-testnet/data/
```

#### Update Your Node ; 

```bash
aztec-up alpha-testnet
```
#### Restart Your Node ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP
```



## 22.05.2025 Update : 

```bash
screen -r aztec
```
- CTRL + C - Stop your Node

#### Delete Your Database 

```bash
rm -rf ~/.aztec/alpha-testnet/data/
```

#### Update Your Node ; 

```bash
aztec-up alpha-testnet
```
#### Restart Your Node ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP
  --p2p.maxTxPoolSize 1000000000
```

## 02.06.2025 Update : 

```bash
screen -r aztec
```
- CTRL + C - Stop your Node

#### Delete Your Database 

```bash
rm -rf ~/.aztec/alpha-testnet/data/
```

#### Update Your Node ; 

```bash
aztec-up latest
```
![image](https://github.com/user-attachments/assets/04718d54-51d2-41c3-8ead-ee2705eaf254)

#### Restart Your Node ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP
  --p2p.maxTxPoolSize 1000000000
```


