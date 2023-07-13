# SolidityAssessment

This file is all about the final project of ETH PROOF: Beginner EVM Course. 

## PROJECT: Create A Token

This code will show us how to mint our first ever token, and how to burn it afterwards.

## Creating The Program

Go to https://remix.ethereum.org/ a online IDE to create our Program

# Executing Program

## The Minting Progress

 function mint(address your_adress, uint add_value)public {
        totalsupply += add_value;
        balances[your_adress] += add_value;
    }

We Create a Function with a purpose of Minting the Token thus we called it Minting
We will get the address with a value of _add and a none negative number for the value of our token

the totalsupply will show us the total supply of our token after minting 
the balance will show us the total balance of token in our address minting

## The Burning Progress

 function burn(address your_adress, uint burn_value)public {
        if(balances[your_adress]>=burn_value){
            totalsupply -= burn_value;
            balances[your_adress] -= burn_value;
        }
 We Create a Function with a purpose of Burning the token thus we called it Burning
 We will get the address with a value of _add and a none negative number for the value of our token

 the totalsupply will show us the total supply of our token after doing the burning process
 the balance will show us the total balance of the token in our address after burning process
