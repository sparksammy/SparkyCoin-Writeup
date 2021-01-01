# SparkyCoin-Writeup
## An automated, digital, unstable fiat-like currency made in NodeJS and Express.js with a so-simple-its-genius design

### Automated
* Automated growth, can "print" more money automatically as circulation grows
  * Starting at 250000 total coins
  * Down to 10 digits behind the decimal point
* Automated transaction tax of 0.5% or at least 0.00001, and at most 0.01 SPARKY to support the creator (Sparksammy)

## Digital, unstable, and fiat-like
* Mining in a different way.
  * Since this is fiat, we do not need "mining" in a typical sence.
  * So we instead have a faucet of sorts, basically you do a simple math equation, you click a button, and it mines a random amount of SparkyCoin
* Wallets are different, too!
  * Since we don't have banks, and we are fiat, you just send the money to someones wallet via their address, and then it's just there!
  * No private keys per-say, instead we use a randomly generated password!
* Everything done via Express.js and NodeJS via an API.
* Unstable as in the value fluctuates, fiat-like as in it's backed by the people.
* There's 1 Database using sqlite3, it only holds: Current amount of coins in wallet, public, and private keys.
