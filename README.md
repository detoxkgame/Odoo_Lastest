# Odoo_Lastest

### Odoo Nightly
```
curl https://nightly.odoo.com/15.0/nightly/windows/odoo_15.0.latest.exe --output odoo_15.0.lastest.exe
curl https://nginx.org/download/nginx-1.20.2.zip --output nginx-1.20.2.zip
curl https://dl.eff.org/certbot-beta-installer-win32.exe --output certbot-beta-installer-win32.exe
curl https://www.python.org/ftp/python/3.10.2/python-3.10.2-amd64.exe --output python-3.10.2-amd64.exe
```

### Commands
```
python -m pip install --upgrade pip
```
```
pip install setuptools wheel
```
```
pip install -r requirements.txt
```

### Bin
```
python odoo-bin -d odoo15 -r <pgadmin_user> -w <pgadmin_pw>
```

### Edit requirements
```
python-stdnum==1.16
libsass==0.21.0
passlib==1.7.2
```

### Links
https://github.com/wkhtmltopdf/wkhtmltopdf/releases/
https://www.python.org/ftp/python/3.10.2/python-3.10.2-amd64.exe


### PowerShell command
Install SSH windows server 2016
```Add-WindowsCapability -Online -Name OpenSSH.Server*```

Test SSH 
```Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Server*'```
Name : OpenSSH.Server ~~~~ 0.0.1.0
State : Installed

Uninstall SSH windows server 2016
```Remove-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0```


