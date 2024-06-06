# foundry-starter-example
Get started with Foundry easily friendly for developers of all knowledge levels to quickly build and deploy SmartContract. (https://book.getfoundry.sh/)

<br/>

<p align="center">
  <a href="https://linktr.ee/nid_z">
      <picture>
        <img alt="logo" src="https://github.com/nidz-the-fact/foundry-starter-example/blob/main/nidz-the-fact-cover.png" width="100%" height="400">
      </picture>
</a>
</p>

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

### Documentation
https://book.getfoundry.sh/

### Install
Git: https://www.git-scm.com/
PowerShell: https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4
or PowerShell(vs-code extension)
*for Windows*

## 1. Starter

### 1.1 install first time

```shell
curl -L https://foundry.paradigm.xyz | bash
```
*cc. learning: https://book.getfoundry.sh/getting-started/installation*
### 1.2 your create foundry

```shell
forge init {NAME_FOLDER}
```
*cc. learning: https://book.getfoundry.sh/getting-started/first-steps*
### 1.3 install inport - openzeppelin

```shell
forge install Openzeppelin/openzeppelin-contracts --no-commit
```
*cc. learning: https://book.getfoundry.sh/projects/dependencies*

## 2. Usage

### 2.1 Clone

```shell
git clone https://github.com/nidz-the-fact/foundry-starter-example
```
### 2.2 Import

```shell
forge install Openzeppelin/openzeppelin-contracts --no-commit
```
*cc. learning: https://book.getfoundry.sh/projects/dependencies*
### 2.3 SmartContract 

```shell
your in src/.. (TestToken.sol)
```
### 2.4 Deploy

```shell
forge create --rpc-url {YOU_RPC_CHAIN} --private-key {YOU_PRIVATE_KEY} src/{YOU_PATH_CONTRACT}:{YOU_NAME_IN_CONTRACT}
```
if there are Arguments add `--constructor-args` {YOUR_ARGS_1_2}
*cc. learning: https://book.getfoundry.sh/reference/forge/forge-create*
### 2.5 Verify

```shell
forge verify-contract --verifier blockscout --verifier-url --rpc-url {EXP_URL}/api? --private-key {YOU_CONTRACT} {YOU_NAME_IN_CONTRACT} --chain-id {CHAIN_ID}
```
if there are Arguments add `--constructor-args` $(cast abi-encode "constructor(string,string)" "TestToken" "TT")
*note: Verification requires importing the file into `src/..` or redeploying it through **foundry**.*
*cc. learning: https://book.getfoundry.sh/reference/forge/forge-verify-contract*
### 2.6 Advance deploy+verify

```shell
forge create --rpc-url {YOU_RPC_CHAIN} --private-key {YOU_PRIVATE_KEY} src/{YOU_PATH_CONTRACT}:{YOU_NAME_IN_CONTRACT} --verify --verifier blockscout --verifier-url {EXP_URL}/api? --chain-id {CHAIN_ID}
```
*note: Verification requires importing the file into `src/..` or redeploying it through **foundry**.*

#

## Commands

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

---

💻💖☕ by [Nidz The Fact](https://linktr.ee/nid_z) 🙏
```
0x361ef0829E71b3bBc806C224ffcecc97813f93cB
```
