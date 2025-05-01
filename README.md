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

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=FurkanL0&style=flat-square&color=red&label=Profile+Views+/+Repo+Views+" alt="Repo / Profile Views" />
</p>
