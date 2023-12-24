[[JWT]]

# Fix secret key must have a value in JWT
#resource 
```.env
JWT_SECRET = my-32-character-ultra-secure-and-ultra-long-secret
JWT_EXPIRES_IN=90
```
[Reference](https://stackoverflow.com/a/62095056)