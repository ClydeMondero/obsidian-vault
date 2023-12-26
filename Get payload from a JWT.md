[[JWT]]

# Get payload from a JWT
#resource 

```javascript
const decoded = jwt.verify(token, "your secret or key");  
var userId = decoded.id  
console.log(userId) 
```

[Reference](https://stackoverflow.com/a/56754095)