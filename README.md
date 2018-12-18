# dapi-mobile-example


移动端dAPI规范文档包括唤醒、扫码、钱包中打开H5 DApp三种场景。详细请看[dAPI for Mobile Specification](dAPI-for-Mobile.mediawiki)

## 钱包中打开H5 DApp场景

1. Open DApp in Provider
2. Get account or get identity
3. Login DApp
4. DApp Invoke smart contract

![](images/scenario3.png)

### Open DApp in Provider

钱包中打开DApp：http://101.132.193.149:5000/#/

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/01-open-dapp.jpg" height="350" width="200">
</div>

### Get account or get identity

DApp登录如果不需要验证用户身份，直接查询账号或身份信息：

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/02-getAccount.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/04-logined.jpg" height="350" width="200">
</div>

### Login DApp

DApp登录如果需要验证用户身份: DApp发消息到给钱包签名，DApp验证签名。

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/03-login-message.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/input-password.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/04-logined.jpg" height="350" width="200">
</div>

### DApp Invoke smart contract

DApp调用合约，用户签名后预执行合约，用户确认并发送交易，返回交易hash给DAPP。

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/05-invoke-message.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/input-password.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/05-pre-exec-result.jpg" height="350" width="200">
   <img src="https://raw.githubusercontent.com/ontio-community/dapi-mobile-example/master/images/ios/06-dapp-recv-txhash.jpg" height="350" width="200">
</div>


## 唤醒、扫码场景


### 登录、调用智能合约

![](images/split-login-invoke.png)

### 未登录时调用智能合约

![](images/invoke-with-login.png)
