# ssh-key

Set Key="C:\Path\to\keyfile"

 Cmd /c Icacls %Key% /c /t /Inheritance:d

 Cmd /c Icacls %Key% /c /t /Grant %UserName%:F

 Cmd /c Icacls %Key% /c /t /Remove Administrator "Authenticated Users" BUILTIN\Administrators BUILTIN Everyone System Users


 Cmd /c Icacls %Key%
 
 # Nginx
 
sudo apt update
sudo apt install nginx

sudo ufw enable

sudo ufw app list

sudo ufw allow 'Nginx HTTP'

sudo ufw status

systemctl status nginx


