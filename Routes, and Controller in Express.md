[[Express]]

# Routes and Controller in Express
#resource 

## bookController.js
```js
const Book = require("../models/book");
const asyncHandler = require("express-async-handler");

exports.book_list = asyncHandler(async (req, res, next) => {
  res.send("NOT IMPLEMENTED: Book list");
});
```

## bookRoute.js 
```js
const express = require("express");
const router = express.Router();

const book_controller = require("../controllers/bookController");

router.get("/book/create", book_controller.book_create_get);

module.exports = route;
```

[Reference](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/routes) 
