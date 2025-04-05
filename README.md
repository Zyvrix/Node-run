# Seismic-Devnet-Contract-Deploy-Guide

Guide to Deploy and Interact with Seismic Devnet Encrypted Contract

---

## ⚙️ Pre-Requirements

### 1. Install Rust

curl https://sh.rustup.rs -sSf | sh  
. "$HOME/.cargo/env"

Verify Installation

bash
Copy
Edit
rustc --version
2. Install jq
For WSL/Ubuntu:

bash
Copy
Edit
sudo apt install jq
For Mac:

bash
Copy
Edit
brew install jq
3. Install sfoundryup
bash
Copy
Edit
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
source ~/.bashrc
4. Run sfoundryup
bash
Copy
Edit
sfoundryup
🔺 This process can take a while to fully download

🚀 Deploy an Encrypted Contract 🎶
1. Clone & Navigate to The Repo
bash
Copy
Edit
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git
cd try-devnet/packages/contract/
2. Deploy Contract
bash
Copy
Edit
bash script/deploy.sh
✅ This script will:

Generate a wallet

Prompt a Faucet URL and the wallet address

You need to fund the wallet using the Faucet — and you're done!

🤖 Interact with an Encrypted Contract
1. Navigate to Home Directory
bash
Copy
Edit
cd $HOME
2. Install Bun
bash
Copy
Edit
curl -fsSL https://bun.sh/install | bash
3. Install Node Dependencies
bash
Copy
Edit
cd try-devnet/packages/cli/
bun install
4. Send Transactions
bash
Copy
Edit
bash script/transact.sh
