[[React]] [[Express]]

# Proxy port for React and Express servers to work
#resource 

```javascript
SERVER:
app.listen(4000, () => console.log("server is up on -p 4000")
```

```javascript
CLIENT:
In the react app package.json file insert this key/value:
{
...
"proxy": "http://localhost:4000",
...
}
```

[Reference](https://stackoverflow.com/a/71392869)