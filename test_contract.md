# Test contract - check if everything is installed correctly

In this step we'll run test contract and this way chack if everything works fine. You'll see what path is being used to test contracts.

## Test deploy of a contract

Comming together with neo-local there is already one smart contract, that we'll use to test whole setup.

1.  within NEO console `neo>` launch command:  
    `build /smart-contracts/wake_up_neo.py test 07 05 True False main`

**CONGRATULATIONS** You have just test deployed your first smart contract into your private blockchain.
    
## Localization of test smart contract

Test contract is within folder on your machine `<path to repo>/neo-local/smart-contracts`

Save your contracts into that folder to test them within private network.


## Useful links

* Contract arguments and returned values  
    <https://neo-python.readthedocs.io/en/latest/data-types.html#contractparametertypes>
* neo-python docs:  
    <https://neo-python.readthedocs.io/en/latest/>
* neo-boa (python 2 neo bytecode compiler)
    
* neo-local
    <https://github.com/neoauth/neo-local>