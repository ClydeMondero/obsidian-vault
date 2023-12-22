[[Powershell]]

# Shorten directory prompt in Powershell
#resource 

Run `powershell` as **administrator**, then run the following:

`Test-Path $Profile`

if it returns `false` then no you don’t have a profile file yet, so create it:

`New-Item –Path $Profile –Type File –Force`

(this will create profile file, or will overwrite the existing one)

Then, edit your profile file:

`notepad $Profile`

Put the function below and save.
```shell
function prompt {'PS ' + $(Get-Location | Split-Path -Leaf) + ">"}
```


[Reference](https://stackoverflow.com/questions/42862604/powershell-shortened-the-directory-prompt-but-how-to-save-the-change)