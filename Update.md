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
```
