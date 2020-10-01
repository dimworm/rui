# Rui锐

Rui is a RChain light wallet, which is a Chrome extension. The purpose of Rui is to let users import Ethereum Keystore, check REV balance and transfer REV.

## Security:
Rui is safe in that you don't lose control of your own key. Your keystore has a password, and further more your login password is used to encrypt your keystore when it is stored in web browser.

## Attention:
Rui is not an ideal place to store your key because it's just a plugin. You have to backup your key somewhere else.

## _Special Thanks to Tomislav for his great work [**@tgrospic/rnode-grpc-js**](https://github.com/tgrospic/rnode-grpc-js)_

# 中文说明 Chinese description:
Rui锐钱包是专门为RChain服务的一款轻钱包，是一个浏览器插件，可与Chrome、360浏览器、百度浏览器、猎豹浏览器、搜狗浏览器、QQ浏览器等配合使用。

## 设计初衷：
RChain主网即将上线。大家手里的私钥都是在以太坊钱包里生成的，所以如何用原有私钥在RChain主网上进行账户余额查询和转账是首先要面对的问题。Rui锐钱包就是要解决这个问题。

## Rui锐钱包能：
1. 导入以太坊keystore
2. 查询账户余额
3. 转账

## Rui锐钱包不能：
浏览器插件使用非常方便，但是牺牲了一些安全性，比如浏览器插件可能会被轻易地删除。所以浏览器插件并不适合于存放私钥。用户首先需要保证自己的私钥在其它地方安全存储，而Rui锐钱包中的存储只是暂时的。

## 安全设计：
为保证私钥在Rui锐钱包中的安全，Rui锐钱包设置有两道密码，第一道是用户的Keystore密码，用户每次查询余额或转账都需要输入该密码；第二道密码是Rui锐钱包的登录密码，该密码还被用于对Keystore的二次加密，用于加强浏览器存储空间的安全性。

## 什么是Keystore?
是以太坊私钥的一种存放方法，是由密码保护的文件。Imtoken, Metamask, Parity, Geth等以太坊钱包都可以导出Keystore。Keystore的优点是有密码保护，比较安全。
