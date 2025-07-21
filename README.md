1. Install prerequisites and updates
``` bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y build-essential pkg-config libssl-dev git-all protobuf-compiler curl
```

2.  Install Rust
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```


3.  Clone the Nexus CLI Repository
```bash
git clone https://github.com/nexus-xyz/nexus-cli.git
cd nexus-cli/clients/cli
```


4.  Build the CLI
```bash
cargo build --release
```
After success, the CLI binary will be located at:
```bash
./target/release/nexus-network
```

5.  Register Your Nexus User and 
   Get your wallet address from the nexus website
```bash
./target/release/nexus-network register-user --wallet-address 0xYourWalletAddress
```

6.  Register Your Node
```bash
./target/release/nexus-network register-node
```

6.  Create Screen
```bash
screen -S bc
```


7.  Start Proving
```bash
./target/release/nexus-network start
```


ENJOY and give star to this repository 

