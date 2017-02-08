# wxaencrypt

An easy-to-use encryption system utilizing RSA and AES for wechat app. 

## Useing

```javascript
//page.js
let cryptico = require('../../utils/cryptico.js');



const MattsPublicKeyString = "uXjrkGqe5WuS7zsTg6Z9DuS8cXLFz38ue+xrFzxrcQJCXtVccCoUFP2qH/" +
"AQ4qMvxxvqkSYBpRm1R5a4/NdQ5ei8sE8gfZEq7dlcR+gOSv3nnS4/" +
"CX1n5Z5m8bvFPF0lSZnYQ23xlyjXTaNacmV0IuZbqWd4j9LfdAKq5dvDaoE=";
var PlainText = "123456";
var EncryptionResult = cryptico.encrypt(PlainText, MattsPublicKeyString);
console.log(EncryptionResult);

```


Fork from [https://github.com/wwwtyro/cryptico](https://github.com/wwwtyro/cryptico)