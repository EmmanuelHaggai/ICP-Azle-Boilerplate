# ICP Azle Boilerplate
 This is a boilerplate repository to streamline development with the ICP Azle framework. This repository is tailored for seamless integration with the message board canister on the Dacade website thus offering a robust foundation for your decentralized applications.

## Key Features:

1. ICP Azle Compatibility: 
The boilerplate code is intricately crafted to align perfectly with the ICP Azle framework, ensuring optimal performance and adherence to best practices.

2. Message Board Canister Integration: 
This repository is designed with a specific focus on compatibility with the message board canister on the Dacade website. Harness the power of the ICP network while effortlessly incorporating message board functionality into your decentralized applications.

## Getting Started:
1. Install dependencies
Ubuntu/WSL
```bash
sudo apt update
sudo apt upgrade
```
```bash
sudo apt install clang
sudo apt install build-essential
sudo apt install libssl-dev
sudo apt install pkg-config
```
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Mac

```bash
# Install the Xcode Command Line Tools
xcode-select --install
```
2. Install Node.js
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
Now restart your terminal and run the following command:
```bash
nvm install 18
```
Check that the installation went smoothly by looking for clean output from the following command:
```bash
node --version
```

3. Install dfx
Run the following command to install dfx 0.15.1:
```bash
DFX_VERSION=0.15.1 sh -ci "$(curl -fsSL https://sdk.dfinity.org/install.sh)"
```
Restart the terminal and then check that the installation went smoothly by looking for a clean output from the following command:
```bash
dfx --version
```
If after trying to run dfx --version you encounter an error such as dfx: command not found, you might need to add $HOME/bin to your path. Here's an example of doing this in your .bashrc:
```bash
echo 'export PATH="$PATH:$HOME/bin"' >> "$HOME/.bashrc"
```
5. clone this repo
```bash
git clone https://github.com/EmmanuelHaggai/ICP-Azle-Boilerplate.git
```
6. Input your custom canister code in src/index.ts

7. Start your dfx code
```bash
dfx start --clean --background
```
8. Deploying your local canister
```bash
dfx deploy
```
After deploying your canister, you will see an output with links that you can use to interact with your canisters.

9. If you want to stop a local replica
```bash
dfx stop
```