# LabZM

*Bitcoin Wallet with Focus on Time Locking Bitcoin*

## Easy Timelocking

LabZM wallet is a simple Electrum format seed compatible wallet, whose main
focus is to enable convenient time-locking of bitcoin. LabZM wallet practically eliminates 
data shuffling and the need for storing data between locking and unlocking. 
Unlocking usually happens long time after locking, and is prone to potentially costly mistakes. 
LabZM allows to unlock funds with only expiration date and time (in addition, of course, to the private keys).

## Unlocking Funds Locked by Other Tools

LabZM wallet can also be used to unlock funds locked by some other tool or wallet, 
you can use the "unlock funds" button which will give you a chance to enter necessary data.

## Lightweight Stateless Wallet

LabZM wallet communicates exclusively with Electrum servers, it does not store the seed nor 
does it have any disk memory. Once it exits, the entire session is forgotten (only during beta test
phase a log file is created at ~/Library/Logs/LabZM/labzm.log - this will be removed
in production version).

## Can be Used as Transaction Generator 

LabZM displays transactions in hexadecimal format before it broadcasts them, 
so you can use it for transaction generation only if you wish (by cancelling broadcasting steps). 
You can easily copy and paste transactions and broadcast them some other way, 
or decode them online to inspect them).

## Address Orientation

LabZM wallet lets you create transactions on particular addresses, in addition to wallet-scoped
operations. Wallet makes it ease to transfer funds between addresses of the same wallet, or
pay from a given address in a wallet. Time-locking also can be performed on wallet-scoped funds
and on funds from a particular address.

## Limitations

Currently, LabZM wallet supports only legacy bitcoin addresses and is only available on Mac.
Segwit and taproot versions are planned asap.

Time-locking has the following limitation - you cannot time-lock more funds than the
largest address in the wallet. If you need to timelock more funds than the largest address
in your wallet, you need to transfer funds between addresses to create big enough address. 
It is easy to make such transfers with LabZM.

## Demo

Please have a look at demonstration video at: https://youtu.be/7oNQKWGYkwk