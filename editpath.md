# Path Reads and Edits

Return Path:
ex: code

```PowerShell
(gcm code).Path
```

```bash
whereis code
```

Raw String:

```PowerShell
echo $env:path
```

```bash
echo $PATH
```

Listed String:

```PowerShell
echo $env:path -split ';'
```

Refresh Path:

Temporary:

```PowerShell
$env:path = [System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")
```

```PowerShell
$env:path= $env:path + ";C:\path\to\bin"
```

https://superuser.com/questions/886951/run-powershell-script-when-you-open-powershell/1009553#1009553

```bash
export PATH=$PATH:"/path/to/bin"
```

Edit Environment Variables when Control Panel locked out:

```PowerShell
rundll32 sysdm.cpl,EditEnvironmentVariables
```

Permanent:

```bash
code ~/.bashrc
```

Paste
`export PATH=$PATH:"/path/to/bin"`

Save and
```bash
source ~/.bashrc
```

Configure Embedded Python:

Make directory to hold it
Change to it

```bash
curl -o filename.zip https://www.python.org/ftp/python/3.12.8/3.12.8-embed-amd64.zip
unzip filename.zip
```

Add directory to python.exe to PATH on PowerShell and GitBash
