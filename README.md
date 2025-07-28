# octraguide


    If you are starting new do this before proceeding for Task 3

    Generate Wallet - Guide
    Install CLI - Guide

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

git clone https://github.com/octra-labs/ocs01-test.git

cd ocs01-test

cargo build --release

cp EI/exec_interface.json .

    Copy the wallet.json file from octra_pre_client folder to ocs01-test folder

./target/release/ocs01-test

    Test all functions
