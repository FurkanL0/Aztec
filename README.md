# Aztec

![681363d8655aaa9274d65eff_Testnet Announcement_blog](https://github.com/user-attachments/assets/d2d9a479-5528-486c-abe5-22d9bddb7ee7)

| X        | Minimum              |
|------------------|----------------------------|
| **CPU**          | 8++ |
| **RAM**          | 16++ GB ( 20++ )                    |
| **Storage**      | 1 TB+ NVME GB SDD                   |
| **Network**      | 100 Mbps (1 Gbps+ recommended) |


| Server Provider        | Link              | Features |
|------------------|----------------------------|----------------------------|
| **Contabo**          | [Link](https://www.dpbolvw.net/click-101330552-12454592)                     | Cheap / Paypal  |
| **PQ**      | [Link](https://pq.hosting/?from=627713)                  | Cheap / Crypto Payment |
| **NetCup**          | [Link](https://www.netcup.com/en/?ref=261820) | Cheap / Paypal |

## Project : 
- Twitter : https://x.com/aztecnetwork

## RPC ; 

- Alchemy
- ANKR
- BEACON L1 : CHAINSTACK 
- Public Node ; https://ethereum.publicnode.com/?sepolia

## 1. Server Update : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Install Packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file unzip lz4 -y
```

## 3. Docker ; 

```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
docker version
```

## 4. Install Docker Compose : 

```bash
VER=$(curl -s https://api.github.com/repos/docker/compose/releases/latest | grep tag_name | cut -d '"' -f 4)
curl -L "https://github.com/docker/compose/releases/download/$VER/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker-compose --version
```

## 4. Docker User Permissions

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
```


# Sequencer Node ; 

#### Sequencer ; Sequencers in the Aztec network propose and produce blocks. Sequencers are also responsible for proposing and voting on network upgrades. Participate using consumer hardware.

#### Install Aztec ; 

```bash
bash -i <(curl -s https://install.aztec.network)
```

![image](https://github.com/user-attachments/assets/23b39122-7e2f-4618-9d5f-2645d4f8b2bd)

- y.

![image](https://github.com/user-attachments/assets/9c3e6e45-286a-45b6-bb41-65c91822ad3e)

- y

#### Fresh Shell ; 

```bash
source .bash_profile
```

#### Try ; 
```bash
aztec
```
## Update ; 

```bash
aztec-up alpha-testnet
```
## Aztec Seq ; 

#### Screen ; 

```bash
screen -S aztec
```
```bash
aztec start --node --archiver --sequencer \
  --network alpha-testnet \
  --l1-rpc-urls RPC_URL  \
  --l1-consensus-host-urls BEACON_URL \
  --sequencer.validatorPrivateKey 0xYourPrivateKey \
  --sequencer.coinbase 0xYourAddress \
  --p2p.p2pIp IP
```

- IP ; Server IP
- 0xYourPrivateKey ; Metamask Private key
- RPC_URL ; Sepolia RPC
- BEACON_URL ; Beacon RPC

#### Sepolia ; 

![image](https://github.com/user-attachments/assets/2700bb9d-5f38-4548-82ee-49e8045e46bc)

#### ChainStack Beacon ; 

![image](https://github.com/user-attachments/assets/5a148704-759c-4bf4-a2cb-98807d43a8fd)


## Role ; 

![image](https://github.com/user-attachments/assets/b16a0561-b81d-4fd4-ad03-8e4e296cba5a)


**Step 1: Get the latest proven block number:**
```bash
curl -s -X POST -H 'Content-Type: application/json' \
-d '{"jsonrpc":"2.0","method":"node_getL2Tips","params":[],"id":67}' \
http://localhost:8080 | jq -r ".result.proven.number"
```
* Save this block number for the next steps
* Example output: 12345

**Step 2: Generate your sync proof**
```bash
curl -s -X POST -H 'Content-Type: application/json' \
-d '{"jsonrpc":"2.0","method":"node_getArchiveSiblingPath","params":["BLOCK_NUMBER","BLOCK_NUMBER"],"id":67}' \
http://localhost:8080 | jq -r ".result"
```
* Replace 2x `BLOCK_NUMBER` with your number

**Step 3: Register with Discord**
* Type the following command in this Discord server: `/operator start`
* After typing the command, Discord will display option fields that look like this:
* `address`:            Your validator address (Ethereum Address)
* `block-number`:      Block number for verification (Block number from Step 1)
* `proof`:             Your sync proof (base64 string from Step 2)

![image](https://github.com/user-attachments/assets/16af82f7-f5d9-4829-9cf1-1cb1f4920fb6)

- DC 
- /operator start 

![image](https://github.com/user-attachments/assets/857c7722-7d46-4406-a027-f87f444aad60)


## Validator Reg
```bash
aztec add-l1-validator \
  --l1-rpc-urls RPC_URL \
  --private-key your-private-key \
  --attester your-validator-address \
  --proposer-eoa your-validator-address \
  --staking-asset-handler 0xF739D03e98e23A7B65940848aBA8921fF3bAc4b2 \
  --l1-chain-id 11155111
```
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=FurkanL0&style=flat-square&color=red&label=Profile+Views+/+Repo+Views+" alt="Repo / Profile Views" />
</p>
