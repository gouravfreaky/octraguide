# Octra Testnet Guide

## TASK 1 : Generate OCTRA Wallet
- Open [CodeSpace](https://github.com/codespaces)
- Select Blank Template
---
### Clone Repository
```
git clone https://github.com/octra-labs/wallet-gen.git
```
```
cd wallet-gen
```
### Install Bun
```
curl -fsSL https://bun.sh/install | bash
```
```
source ~/.bashrc
```
```
bun install
```
```
bun run build
```
```
bun start
```
- A pop-up will appear so click on it to open the local host browser
- Generate Wallet & Save Everything
- Get [Faucet](https://faucet.octra.network) (Sometimes it doesn't work)

---
## Task 2 - Transfer Tokens
- Create New [Codespace](https://github.com/codespaces)

### Install CLI
```
git clone https://github.com/octra-labs/octra_pre_client.git
```
```
cd octra_pre_client
```
```
pip install -r requirements.txt
```
```
cp wallet.json.example wallet.json
```
```
nano wallet.json
```
* Replace following values:
  * `private-key-here`: Privatekey with `B64` format (already saved earlier)
  * `octxxxxxxxx...`: Octra address starting with `oct...`
* Use CTRL X Y & Enter to Exit

```
./run.sh
```
<img width="1095" height="666" alt="image" src="https://github.com/user-attachments/assets/192cdea6-9f51-4aba-ab44-863aad433247" />

- Use the UI to send trx to address
- Address to send: `octEXhrh986DtwJFY3qG3ANsrV63TP7zorxybB8EGMStr81`

## Task 3 - Encrypted Transactions
- Create New [Codespace](https://github.com/codespaces)

### Install CLI
```
git clone https://github.com/octra-labs/octra_pre_client.git
```
```
cd octra_pre_client
```
```
pip install -r requirements.txt
```
```
cp wallet.json.example wallet.json
```
```
nano wallet.json
```
* Replace following values:
  * `private-key-here`: Privatekey with `B64` format (already saved earlier)
  * `octxxxxxxxx...`: Octra address starting with `oct...`
* Use CTRL X Y & Enter to Exit

```
./run.sh
```
<img width="1095" height="666" alt="image" src="https://github.com/user-attachments/assets/192cdea6-9f51-4aba-ab44-863aad433247" />

- Now let's select different options from the UI and test them.
- You can test your first trx on this address: `octEXhrh986DtwJFY3qG3ANsrV63TP7zorxybB8EGMStr81`

## Task 4 - OCS01 Test Contract
- If you are starting new do this before proceeding for Task 3
1. Generate Wallet - [Guide](https://github.com/colonyairdrops/Octra#generate-octra-wallet)
2. Install CLI - [Guide](https://github.com/colonyairdrops/Octra#install-cli)

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
```
source $HOME/.cargo/env
```
```
git clone https://github.com/octra-labs/ocs01-test.git
```
```
cd ocs01-test
```
```
cargo build --release
```
```
cp EI/exec_interface.json .
```
- Copy the `wallet.json` file from octra_pre_client folder to ocs01-test folder
```
./target/release/ocs01-test
```
* Test all functions


---
- Follow me on X - https://x.com/erbagoragourav
