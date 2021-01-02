# SparkyCoin-Writeup
## An automated, digital, unstable fiat-like currency made in NodeJS and Express.js with a so-simple-its-genius design

### Automated
* Automated growth, can "mint" more money automatically as circulation grows
  * Starting at 250000 total coins
  * Down to 19 digits behind the decimal point

## Digital, unstable, and fiat-like
* Mining in a different way.
  * Since this is fiat, we do not need "mining" in a typical sence.
  * So we instead have a faucet of sorts, but with a guessing game, where you guess the sum of two numbers you don't know. These two numbers range from one to 12, and these two numbers only last for 1 GET request.
* Wallets are different, too!
  * Since we don't have banks, and we are fiat, you just send the money to someones wallet via their address, and then it's just there!
* Everything done via Express.js and NodeJS via an API.
* Unstable as in the value fluctuates, fiat-like as in it's backed by the people.
* There's 2 Databases using Quick.db, they only hold: Current amount of coins in wallet, public, private keys, and currently "minted" coins.

## Centrally Decentralized.
* Decentralized meaning there are servers everywhere
* Centrally meaning that each server hosts their own database
 * With their own data.
 
### Most importantly, people don't have to ask for a fork. Fork Freely.
