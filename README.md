## REMIX ETHEREUM - CREATING TOKENS

# Description
This Solidity application shows the fundamental syntax and capabilities of the Solidity programming language by demonstrating how to create tokens, remove tokens to specific addresses, and restore balances. The goal of this program is to give individuals who are unfamiliar with Solidity a place to start learning about it.

# Getting Started
Written in Solidity, a programming language used to create smart contracts on the Ethereum blockchain, this application is a straightforward contract that demonstrates the creation procedure for a token. The function of creating new tokens or coins, removing existing ones, and displaying addresses and balances are all contained in the contract.

# Executing the program 
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
// SPDX-License-Identifier: MIT
- So, First we started on public variables such as tokenName, tokenAbbreviation and total supply
- Second we need to address the mapping variables because mapping variables is use to track the balance of each address in the contract.
- third is the mint function as you can see the codes there are positive signs because that is used to create new token within a blockchain.
- last is that burn function this is the opposite of mint function as you can see the there are negative signs because that is used to remove a certain number of token.
pragma solidity 0.8.18;

contract MyToken {

    // public variables here

    string public tokenName + "META";
    string public tokenAbbrev = "MTA";
    uint public totalSupply = 0;

    // mapping variable here

    mapping(address => uint) public balances;

    // mint function

function mint (address _address, uint _values) public {
	totalSupply += _value;
	balances[-address] += _value;
}

    // burn function

    
function burn (address _address, uint _values) public {
	if(balances [_address] >=_value) { 
	totalSupply -= _value;
	balances[_address] -= _value;
}

}

}

Lastly we need to compile the contract in the Remix Ethereum IDE too, just because to see the function of every variables
and we need to deploy every variables to the function 
