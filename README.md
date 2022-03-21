# Odoo_Lastest version windows64

## Odoo Nightly

### Download Links 
Git x64[2.35.1.2]https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe)

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
pandas==0.20.3
```




### PowerShell command
Install SSH windows server 2016
```Add-WindowsCapability -Online -Name OpenSSH.Server*```

Crear regla en el firewall para SSH en el puerto 22
```New-NetFirewallRule -Name sshd -DisplayName 'OpenSSH Server (sshd)' -Enabled True -Direction Inbound -Protocol TCP -Action Allow -LocalPort 22```


### PSQL command

White screen after log in
```DELETE FROM ir_attachment WHERE name SIMILAR TO '%.(js|css)'; ```

PG_dump 
```
set PGPASSFILE="<dir_pgpass.conf>"
pg_dump -h <host> -p <port> -U <user> -F c -b -v -f "<dir_file.backup>" <database>
```
PG_restore
```
pg_restore -h <host> -p <port> -U <user> -d <database> -v "<dir_file.backup>"
```

.pgpass format: hostname:port:database:username:password

### Bin
```
python odoo-bin -d odoo15 -r <pgadmin_user> -w <pgadmin_pw>
```


### Links
Install SSH winserv [documantation](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

Configurar [Nginx](https://www.digitalocean.com/community/questions/run-odoo-with-nginx-at-port-80)

Nginx config files [Generator](https://www.digitalocean.com/community/tools/nginx)
