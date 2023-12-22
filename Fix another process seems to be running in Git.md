[[Git]]

# Fix another process seems to be running in Git
#resource 
```powershell
rm -f .git/index.lock
```
[Reference](https://stackoverflow.com/a/38004193)