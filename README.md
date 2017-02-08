# wxaencrypt

An easy-to-use encryption system utilizing RSA and AES for wechat app. 

## Useing

```javascript
//page.js
let wxaencrypt = require('../../utils/wxaencrypt.js');


let encrypt = new JSEncrypt.JSEncrypt();
let plainText = "123456";
encrypt.setPublicKey(`-----BEGIN PUBLIC KEY-----
MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDlOJu6TyygqxfWT7eLtGDwajtN
FOb9I5XRb6khyfD1Yt3YiCgQWMNW649887VGJiGr/L5i2osbl8C9+WJTeucF+S76
xFxdU6jE0NQ+Z+zEdhUTooNRaY5nZiu5PgDB0ED/ZKBUSLKL7eibMxZtMlUDHjm4
gwQco1KRMDSmXSMkDwIDAQAB
-----END PUBLIC KEY-----`);
let encrypted = encrypt.encrypt(plainText);
console.log(encrypted);
```


Fork from [https://github.com/wwwtyro/cryptico](https://github.com/wwwtyro/cryptico)