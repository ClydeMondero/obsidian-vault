[[Vim]]

# Use Vim in Windows Terminal
#resource 

1. Press `Ctrl`+`R` to open the Run command window
2. Type `sysdm.cpl` to open the System Properties window  
    [![enter image description here](https://i.stack.imgur.com/QjqQPm.png)](https://i.stack.imgur.com/QjqQPm.png)
3. Click the _Advanced_ tab
4. Click _Environment Variables..._ button  
    [![enter image description here](https://i.stack.imgur.com/J5Pv4m.png)](https://i.stack.imgur.com/J5Pv4m.png)
5. Choose either _User variable for [Your user name]_ or _System variables_, click the row with `Path` variable
6. Click _Browse..._ to find the Vim executable. If the version of vim installed is 8.2.XXXX, it should be located at _C:\Program Files (x86)\Vim\vim82_, else change the `vim82` into the appropriate folder name where your _gvim.exe_ is located at.

[Reference](https://stackoverflow.com/a/68882740) 