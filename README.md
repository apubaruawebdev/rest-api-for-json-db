## Rest API for JSON DB

```js
const express = require("express");
const colors = require("colors");
const dotenv = require("dotenv").config();

// init environment variable
const PORT = process.env.PORT || 8080;

// init express
const app = express();

// express middlewares
app.use(express.json());
app.use(express.urlencoded({ extended: false }));

// server listen
app.listen(PORT, () => {
  console.log(`Server Running on Port ${PORT}`.bgGreen.black);
});
```
