# Seismic-Devnet-Contract-Deploy-Guide

Guide to Deploy and Interact with Seismic Devnet Encrypted Contract

---

## ⚙️ Pre-Requirements

### 1. Install Rust

curl https://sh.rustup.rs -sSf | sh  
. "$HOME/.cargo/env"

Verify Installation
rustc --version

2. Install jq
For WSL/Ubuntu:

sudo apt install jq
For Mac:

brew install jq
3. Install sfoundryup

curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
source ~/.bashrc

4. Run sfoundryup
sfoundryup
🔺 This process can take a while to fully download

🚀 Deploy an Encrypted Contract 🎶
1. Clone & Navigate to The Repo

git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git
cd try-devnet/packages/contract/

2. Deploy Contract
bash script/deploy.sh

✅ This script will:
Generate a wallet
Prompt a Faucet URL and the wallet address
You need to fund the wallet using the Faucet — and you're done!

🤖 Interact with an Encrypted Contract
1. Navigate to Home Directory
cd $HOME

2. Install Bun
curl -fsSL https://bun.sh/install | bash

3. Install Node Dependencies
cd try-devnet/packages/cli/

bun install
4. Send transactions
bash script/transact.sh
bun install
6. Send Transactions
bash
Copy
Edit
bash script/transact.sh
