## 3. Güncelleme ; 

- Screene girelim.

```bash
screen -r aztec
```

- CTRL + C ' yaparak nodemizi durduruyoruz.

#### Eski Database'i Yok Ediyoruz.

```bash
rm -rf ~/.aztec/alpha-testnet/data/
```

#### Güncellemeyi Atıyoruz ; 

```bash
aztec-up alpha-testnet
```
#### Node Başlatma Komutumuz bu - Yeniden başlatıyoruz ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP
```
