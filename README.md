![Banner Image](http://i.imgur.com/okQTt6q.png)


Installation
---------------------

###NPM:
```
npm i rekrypt --save
```

Documentation
---------------------

###Basic Usage
```javascript
//Import Rekrypt
const rekrypt = require('rekrypt');

//Basic Encryption
//Encrypt takes 3 arguments. 2 of which are optional:
//encrypt('String', 'Key', Timestamp)
var encrypted = rekrypt.encrypt('Hello World!');
//This returns ['Encrypted String', 'key', Timestamp]

//Basic Decryption
//Decrypt takes the same arguments as encrypt
//But the string is the one we want to decrypt.
var decrypted = rekrypt.decrypt(encrypted[0],encrypted[1]);
//Here encrypted[0] is the encrypted string
//And encrypted[1] is the key used to decrypt the message.

console.log(`Encrypted Array: ${encrypted}`);
console.log(`Decrypted String: ${decrypted}`);
```

###Syntax

```javascript
encrypt( "String To Encrypt", "Optional Key", Optional Timestamp );
```

```javascript
decrypt( "String To Decrypt", "Encryption Key", Optional Timestamp );
```

```javascript
makekey( length );
```
