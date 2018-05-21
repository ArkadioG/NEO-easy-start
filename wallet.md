# Portfel 

Wallet is being used to store NEO and GAS, deployment and invocate smart contracts.

After installation of **neo-local** there is available wallet containing:moneybag: :
* **1.000.000 NEO**
* **16 624 GAS** 

## Wallet data

* wallet path: `./neo-privnet.wallet`
* wallet password `coz`


* **WIF key:** `KxDgvEKzgSBPPfuVfw67oPQBSjidEiqTHURKSDL1R7yGaGYAeYnr`
* **Adres:** `AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y`
* **Script hash:** `b'#\xba\'\x03\xc52c\xe8\xd6\xe5"\xdc2 39\xdc\xd8\xee\xe9'`

Explanation:
* WIF - private key of your wallet
* Address - public address of wallet (you can send money to that address)
* Script hash - hashed address - used within contracts as argument to  `CheckWitness` function.

## Opening wallet

Within `neo>` console (after running neo-local):
* open wallet  
    `open wallet ./neo-privnet.wallet`
* rebuild:  
    `wallet rebuild`
* display wallet info:  
    `wallet`
    
## Network fees

Deploying contracts to blockchain demands to pay a fee. You deploy contract using wallet, so that wallet hast to have sufficient funds:
* **100 GAS** - for deploying contract
* **+400 GAS** - for permanent storage
* **+500 GAS** - for dynamic invocation (not usable for now)  

Network takes fees for all instructions done during contract execution. If calculated fees are lower than **10 GAS**, then that execution will be done for free.

>Fees information: <http://docs.neo.org/en-us/sc/systemfees.html>

Private network gets the same fees as main net, so we need wallet with plenty of GAS to test our contract.

 #### [Next Step - test deploy of contract](test_contract.md) 
 