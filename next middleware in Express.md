[[Express]]

# next middleware in Express
#resource 

```javascript
app.get('/hello', function (req, res, next) {
  if(some condition){
    next();
    return;
  }
  res.send("Hello World !!!!");  
});

app.get('/hello', function (req, res, next) {
  res.send("Hello Planet !!!!");
});
```

[Reference](https://stackoverflow.com/a/49387994)