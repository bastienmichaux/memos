# Express

### Setup

```bash
mkdir mydir && cd mydir
npm init -y
npm i -s express
```

### Hello world http://localhost:3000

```js
const express = require('express');
const app = express();
app.get('/', (req, res) => {
  res.send('Hello World!');
});
app.listen(3000, () => {
  console.log('Express web app on localhost:3000');
});
```
