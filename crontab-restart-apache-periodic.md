## Restart apache centos 7 periodically
  
## Spesifikasi pengujian
OS Version : Centos 7.5  

## Langkah-langkah
Login sebagai root  
Edit crontab  
```
crontab -e  
```
Sesuaikan dengan script berikut.  
Pada contoh berikut, waktu yang digunakan pukul 23.59  
```
59 23 * * * /bin/systemctl restart httpd.service  
```  

