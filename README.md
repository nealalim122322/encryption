# Data encryption for Next.js
A simple data encryption that can be use in Next.js

## Installation

```sh
npm i @nealalim122322/encryption
```

## Usage

```jsx
import NealCrypto from "@nealalim122322/encryption";
const crypto = new NealCrypto(process.env.NEXT_PUBLIC_SECRET_KEY);

const encryptedPassword = await crypto.encrypt("YOUR STRING");
console.log(`Encrypted: ${encryptedPassword}`);

const decryptedPassword = await crypto.decrypt(encryptedPassword);
console.log(`Decrypted: ${decryptedPassword}`);
```