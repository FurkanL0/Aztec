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

## 02.06.2025 Günceleme : 

```bash
screen -r aztec
```
- CTRL + C - Nodemizi durduralım

#### Eski Datayı Temizleyelim 

```bash
rm -rf ~/.aztec/alpha-testnet/data/
```

#### Node Güncelleme ; 

```bash
aztec-up latest
```
![image](https://github.com/user-attachments/assets/0bdd9052-64cb-4909-bc6e-9100f5987b57)

## Versiyon Kontrolü : 

```bash
aztec -V
```

- 0.87.6 ve üstü olmalı.


#### Yeniden Başlatalım ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP \
  --p2p.maxTxPoolSize 1000000000
```

## 04.06.2025 Günceleme : 

```bash
screen -r aztec
```
- CTRL + C - Nodemizi durduralım

#### Node Güncelleme ; 

```bash
aztec-up latest
```
![image](https://github.com/user-attachments/assets/72cbd131-e82e-413f-bfd6-5e1fe4f491f9)


## Versiyon Kontrolü : 

```bash
aztec -V
```

- 0.87.7 ve üstü olmalı.


#### Yeniden Başlatalım ; 

```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP \
  --p2p.maxTxPoolSize 1000000000
```
