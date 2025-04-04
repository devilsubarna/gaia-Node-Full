# Gaianet-Node-Run-Full-Guide

## Need Some Software Requirements for PC Users

1. For Windows Install WSL - https://learn.microsoft.com/en-us/windows/wsl/install#install-wsl-command

2. For Windows Install Ubuntu after Installing WSL - https://apps.microsoft.com/detail/9PDXGNCFSCZV?hl=en-us&gl=IN&ocid=pdpshare

3. For macOS If you have Installed Homebrew (https://brew.sh/) to manage packages on OS X,
run this command to install Git.
```
brew install git
```

## Need Some Hardware Requirements [Check Out](system-requirements.md)

## Need to Free Your 8080 Port

Identify the Process Using Port 8080
```
sudo ss -tulpn | grep 8080
```

Example - ``` LISTEN  0  128  0.0.0.0:8080  0.0.0.0:*  users:(("nginx",pid=1234,fd=6)) ```

Terminate the Process by PID
```
sudo kill -9 1234
```

Kill All Processes Using Port 8080
```
sudo fuser -k 8080/tcp
```

## Delete Your Old Gaianet Files
```
rm -rf gaianet
```

## Make Account First

Go:- [https://tinyurl.com/ycyaxm7w](https://www.gaianet.ai/reward?invite_code=RFGQUI)

Refer Code:- RFGQUI

1️⃣ Dependencies for WINDOWS & LINUX & VPS
```
sudo apt update
sudo apt upgrade -y
```

For VPS Only
```
apt install screen -y
```

2️⃣ Download Some Files
```
curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
```
```
source /root/.bashrc
```
```
gaianet init --config https://raw.githubusercontent.com/GaiaNet-AI/node-configs/main/qwen-1.5-0.5b-chat/config.json
```

## 🔶 For VPS Only
```
screen -S gaia
```

3️⃣ Start Node & Stop Node
```
gaianet start
```
```
gaianet stop
```

For VPS Only
```
PRESS CTRL+A+D (to run ur miner continuously)
```

### Solution For PID
Check Your PID List
```
ps
```

Delete Your PID
```
kill 69 [Example - if showing 69]
```

4️⃣ Check Your Node ID & Device ID
```
gaianet info
```

5️⃣ Check Your Points 

Go:- [https://tinyurl.com/ycyaxm7w](https://www.gaianet.ai/reward?invite_code=RFGQUI)

Refer Code:- RFGQUI

## 🔶For Same Day as well as Next Day Run This Command (Windows)

#1 Open WSL and Put this Command 
```
gaianet start
```
