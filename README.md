# DATAGRAM-NETWORK-CLI 🚀

A **Node.js/Go-based command-line tool** to interact with the Datagram network running nodes, managing keys, and handling daily operations like license authentication and node stats. Ideal for developers and testers looking to automate Datagram node workflows.

## FEATURES

- **License Management**: Input full-core or partner-license in CLI or environment variables.
- **Run Nodes**: Start a full or partner core node directly from terminal.
- **Node Monitoring**: Fetch and display current node state, peer connections, and uptime.
- **Config via CLI Flags / Env Vars**: Easy customization on-the-fly.

---

##  Minimum System Requirements

| Component | Requirement |
|-----------|-------------|
| CPU       | 4 Cores     |
| RAM       | 4 GB        |

##  Prepare This Before Installation

| Task | Description |
|------|-------------|
| ✅ VPS | Linux VPS (Ubuntu 20.04 or newer) |
| ✅ Terminal Access | Basic command-line knowledge |
| ✅ Accounts | Discord, Telegram, and X (Twitter) |
| ✅ Dashboard | Registered on Datagram Dashboard |
| ✅ API Key | Get from Wallet > Licenses tab |


## PRE-REQUISITES

Make sure you’ve got these installed:

```bash
sudo apt update
sudo apt install git wget curl -y
```
Download and make the CLI executable:

```bash
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux && \
sudo mv datagram-cli-x86_64-linux /usr/local/bin/datagram-cli && \
sudo chmod +x /usr/local/bin/datagram-cli
```

## Run the Node

First, create a screen session using the following command. This ensures your node keeps running even if you close the terminal:

```bash
screen -S datagram
```

```bash
datagram-cli run -- -key ENTER_API_KEY
```

Replace `ENTER_API_KEY` with the actual key you got from Datagram.

### Now, open the Datagram Dashboard and:

- Go to the Wallet section.

- Click on the Licenses tab (next to "Main").

- Copy your API Key from there.

Then run the following command (make sure to replace YOUR_API_KEY with the actual key you just copied):

### If everything works, you’ll see output like:

```bash
App version: 1.1.x
Downloading...
Worker version: 1.1.x
INFO: Downloaded 100.00%
Run...
34527
```

To detach from the screen (without stopping the process): Press `Ctrl + A`, then `D`

## View Node Logs

To reattach the screen and view live node logs:

```bash
screen -r datagram
```

To detach from the screen (without stopping the process): Press `Ctrl + A`, then `D`


## Confirm Participation

Make sure to fill out the **Early Alpha Form** using your **X (Twitter)** and **Discord** information to officially participate in the Datagram Network Alpha.

Your node will **start earning points after 4~6 hours** of continuous uptime. For **maximum rewards**, keep your node running **24/7** without interruptions.



