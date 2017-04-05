# git_test

# RESTful API

[ More Information](https://www.boscoin.io)

## User sendTransaction

- ### type - sendBOS

 http://localhost:8080/blockchain/transactions/sendTransaction

>#### Request parameter :
```
 sendBOS(type)/sender account address/receiver account address/amount/fee
```
>#### Response parameter :
```
 { "sendBOS" : true }
```

- ### type - sendProposal

 http://localhost:8080/blockchain/transactions/sendTransaction

> #### Request parameter :
```
 sendProposal(type)/sender account address/receiver account address/contents/fee
```
> #### Response parameter :
```
 { "sendProposal" : true }
```

- ### type - sendVote

 http://localhost:8080/blockchain/transactions/sendTransaction

> #### Request parameter :
```
 sendVote(type)/sender account address/receiver account address/contents/fee
```
> #### Response parameter :
```
 { "sendVote" : true }
```

## Account Operation

- ### createSeed

 http://localhost:8080/blockchain/AccountOperations/creatSeed

> #### Request parameter :
```
 Nothing
```
> #### Response parameter :
```
 { "passphrase" : 12 words}
```

- ### confirmSeed

 http://localhost:8080/blockchain/AccountOperations/confirmSeed

> #### Request parameter :
```
 { "passphrase" : 12 words}
```
> #### Response parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX",
   "account balance" : 0,
   "freezing status" : false}
```

- ### getAccount

 http://localhost:8080/blockchain/AccountOperations/getAccount

> #### Request parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```
> #### Response parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX",
   "account balance" : udouble,
   "available balance" : udouble,
   "pending balance : udouble, 
   "freezing status" : bool,
   "freezing amount" : udouble,
   "freezing start time" : uint,
   "freezing interests" : udouble}
```

- ### getBalance

 http://localhost:8080/blockchain/AccountOperations/getBalance

> #### Request parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```
> #### Response parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX",
   "account balance" : udouble,
   "available balance" : udouble,
   "pending balance" : udouble}
```

- ### getFreezingStatus

 http://localhost:8080/blockchain/AccountOperations/getgetFreezingStatus

> #### Request parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```
> #### Response parameter :
```
 { "freezing status" : bool,
   "freezing amount" : udouble,
   "freezing start time" : uint,
   "freezing interests" : udouble}
```

- ### getAccountTransaction

 http://localhost:8080/blockchain/AccountOperations/getAccountTransaction

> #### Request parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```
> #### Response parameter :
```
 { {“type" : "sendBOS/sendProposal/sendVote",
   “timestamp" : uint,
   “amount" : double,
   “fee or reward" : double,
   “accout address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```

- ### delAccount

 http://localhost:8080/blockchain/AccountOperations/delAccount

> #### Request parameter :
```
 { "account address" : "BOS-XXXXX-XXXXX-XXXXXXX"}
```
> #### Response parameter :
```
 { “delAccouint" : true}
```