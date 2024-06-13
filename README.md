# Creating a token
This solidity contract is created to learn by implementing tokens. We learned creating a token, deploying them, minting tokens and burning tokens aswell.



## Description

This smart contract is called MyToken used for creating tokens and using its functionalities. Its funcatonalities include creating a token, minting tokens and burning them and also see the remaining balance in the process. 

## Getting Started

### Installing

To use Mytoken, simply download or clone the solidity contact file attached to this repository.

### Executing program

*To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
Further steps,

1. Compile the MyToken contract on an Ethereum-compatible blockchain. 
2. Deploy the MyToken contract on  an Ethereum compatible blockchain.
3. Now an account address is created for that token copy it and paste it into mint token along with required number of tokens to be minted.
4. You can also check the  balance of token in balance by putt in the account address into it.
5. For burning the tokens insert the account address  and no. of token needs to be burnt then click on transact.
   
   This code will help you by mint tokens, burn tokens and tracking token balance of addresses.

```
// mint function
     function mint(address add, uint val) public{
        totalsupply += val;
        balances[add] += val;
```
```
    // burn function
     function burn(address add, uint val) public{
        if(balances[add] >= val)
        {
            totalsupply -= val;
            balances[add] -= val;
        }
```
## Help

Any advise for common problems or issues.
```
solidity --help
```

## Authors

Atul Sharma  
@ findatul.sharma@gmail.com


## License

This project is licensed under the MIT License - see the LICENSE.md file for detail.
