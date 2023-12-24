[[Powershell]]

# Run an exe file if not already running in Powershell
#resource 

```powershell
$Running = Get-Process prog -ErrorAction SilentlyContinue
$Start = {([wmiclass]"win32_process").Create($Prog)} 
if($Running -eq $null) # evaluating if the program is running
{& $Start} # the process is created on this line
```

[Reference](https://stackoverflow.com/a/8834879)