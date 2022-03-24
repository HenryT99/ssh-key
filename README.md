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

# Key SSH
## gen private key for SSH
puttygen -t rsa -b 2048 -o private.ppk

## convert ppk to pem
puttygen private.ppk -O private-openssh -o private.pem

## gen public key from private key
openssl rsa -in private.pem -pubout

## gen public key for authorized_key
ssh-keygen -y -f private.pem


## format old private key
openssl rsa -text -in private.key
