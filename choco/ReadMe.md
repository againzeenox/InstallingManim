
## Install `choco`:
#### 1. Run `Windows PowerShell` as `Administrator`
#### 2. Run
```PS
Set-ExecutionPolicy Bypass -Scope Process
```
#### 3. Run 
``` PS
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
#### 4. Run `choco` or `choco -?` to test the Installation
