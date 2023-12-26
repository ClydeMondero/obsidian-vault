[[Express]]

# Handling cookies in Express
#resource 

```javascript
const express('express')
    , cookieParser = require('cookie-parser'); // in order to read cookie sent from client

app.get('/', (req,res)=>{

    // read cookies
    console.log(req.cookies) 

    let options = {
        maxAge: 1000 * 60 * 15, // would expire after 15 minutes
        httpOnly: true, // The cookie only accessible by the web server
        signed: true // Indicates if the cookie should be signed
    }

    // Set cookie
    res.cookie('cookieName', 'cookieValue', options) // options is optional
    res.send('')

})
```

[Reference](https://stackoverflow.com/a/40135050) 