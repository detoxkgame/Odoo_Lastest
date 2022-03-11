# Odoo_Lastest version windows64

## Odoo Nightly

### Download Links 

Odoo [Last version WIN](https://nightly.odoo.com/15.0/nightly/windows/odoo_15.0.latest.exe)

WKHTMLTOPDF[ WIN64](https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox-0.12.5-1.msvc2015-win64.exe)

Python[3.10](https://www.python.org/ftp/python/3.10.2/python-3.10.2-amd64.exe)

[DUC No-IP](https://www.noip.com/client/DUCSetup_v4_1_1.exe)

Nginx[1.20.2.zip](https://nginx.org/download/nginx-1.20.2.zip)

[Build Tools para Visual Studio 2022](https://aka.ms/vs/17/release/vs_BuildTools.exe)


`curl https://dl.eff.org/certbot-beta-installer-win32.exe --output certbot-beta-installer-win32.exe`




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



### Edit requirements
```
python-stdnum==1.16
libsass==0.21.0
passlib==1.7.2
```




### PowerShell command
Install SSH windows server 2016
```Add-WindowsCapability -Online -Name OpenSSH.Server*```

Test SSH 
```Get-Service -Name *ssh*```

~~Uninstall SSH windows server 2016~~
```Remove-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0```

Crear regla en el firewall para SSH en el puerto 22
```New-NetFirewallRule -Name sshd -DisplayName 'OpenSSH Server (sshd)' -Enabled True -Direction Inbound -Protocol TCP -Action Allow -LocalPort 22```

Conectarse por tunel SSH
```ssh -p 22 admin@<windows_IP>```





### Bin
```
python odoo-bin -d odoo15 -r <pgadmin_user> -w <pgadmin_pw>
```
