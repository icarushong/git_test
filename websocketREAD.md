## Websocket Transaction for Web User Interface 
### - Event Data from Core to UI front

## Table of Contents

  - [User receiveTransaction](#user-receivetransaction)
    - [receiveBOS](#type---receivebos)
    - [receiveProposal](#type---receiveproposal)
    - [sendVote](#sendvote)
  - [Account Operations](#account-operations)
    - [createSeed](#createseed)
    - [confirmSeed](#confirmseed)
    - [getAccount](#getaccount)
    - [getBalance](#getbalance)
    - [getFreezingStatus](#getfreezingstatus)
    - [getAccountTransaction](#getaccounttransaction)
    - [delAccount](#delaccount)
 

## User receiveTransaction

- ### type - receiveBOS

>#### Receive parameter :
```
string receiveBOS, 
string receiver account address, 
string sender account address, 
udouble amount
```

- ### type - receiveProposal

>#### Receive parameter :
```
string receiveProposal, string receiver account address, string account address, string contents
```

