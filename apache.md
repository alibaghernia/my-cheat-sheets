# Apache

## Reload Apache
```bash
sudo systemctl reload apache2
sudo service apache2 reload
```

## laravel priject coonf file
```
<VirtualHost *:80>
    ServerName domain.ir
    ServerAlias www.domain.ir
    ServerAdmin info@domain.ir
    DocumentRoot /var/www/project/public/

    <Directory /var/www/project/public/>
            AllowOverride All
#            Require all granted
#            Options Indexes FollowSymLinks
#            Require all granted

    </Directory>

    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
```
