### zema-dev-task

## Zama Developer Program – Level 2 & 3 Guide
Complete Level 2 and 3 of the Zama Developer Program

## Environment
Windows: Use Linux Ubuntu OS ( Run in admin )

## Install Dependencies
# Packages:
<br>sudo apt update && sudo apt upgrade -y
sudo apt install screen curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y<br>

# Install Nodejs, npm, yarn
<br>sudo apt update
sudo curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -
sudo apt install -y nodejs
node -v
npm install -g yarn
yarn -v<br>

# Install Hardhat:

<br>npm install --save-dev hardhat<br>

# Deploy FHECounter contract
<br>git clone https://github.com/zama-ai/fhevm-hardhat-template
cd fhevm-hardhat-template<br>

# Install:

<br>npm install<br>

# Replace hardhat.config.ts file:

<br>curl -o hardhat.config.ts https://raw.githubusercontent.com/0xmoei/zama-fhe/refs/heads/main/hardhat.config.ts<br>

# Set Sepolia RPC:

<br>npx hardhat vars set SEPOLIA_RPC_URL<br>

# It prompts you to enter a Sepolia RPC, you can use https://ethereum-sepolia-rpc.publicnode.co
Set Privatekey: Use Burner Wallet

<br>npx hardhat vars set PRIVATE_KEY<br>

# It prompts you to enter a privatekey, enter without 0x perfix.
Verify your wallet:

<br>npx hardhat accounts --network sepolia<br>

# Compile and Deploy:

<br># Compile
npx hardhat compile

# Deploy
npx hardhat deploy --network sepolia<br>

# It responds with your deployed contract address
Claim Level 3
Visit: https://guild.xyz/zama/developer-program

→ Find Level 3: Deploy your confidential contract → Paste your deployed contract address

🎉 You’ve completed Level 3!

Made with ❤️ by Morsyxbt
