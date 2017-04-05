# git_test

# RESTful API

- ## sendTransaction

> ### type - sendBOS

```
http://localhost:8080//blockchain/transactions/sendTransaction
```
>>#### Request parameter :
```
sendBOS(type)/sender account address/receiver account address/amount/fee
```
>>#### Response parameter :
```
{ "sendBOS" : true }
```

### type - sendProposal

```
http://localhost:8080//blockchain/transactions/sendTransaction
```
#### Request parameter :
```
sendBOS(type)/sender account address/receiver account address/amount/fee
```
#### Response parameter :
```
{ "sendProposal" : true }
```