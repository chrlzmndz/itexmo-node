# ITEXMO

An SMS library exported as [Node.js](https://nodejs.org/) modules from [ITEXMO](https://itexmo.com/).

## Installing

Using npm:

```shell
$ npm install itexmo-node
```

## Example

In Node.js:

```js
// other parameters: priority String, senderID String, server String
const itexmo = require('itexmo')({
  apiCode: 'YOUR_API_CODE',
  password: 'YOUR_PASSWORD'
});

itexmo
  .send({ to: '+63xxxxxxxxx', body: 'hello world' })
  .then(message => console.log(message));
```
