Virtual Host for linux

<VirtualHost *:80>
    ServerAdmin razzaghi229@gmail.com
    DocumentRoot "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/nad/"
        ServerName nad.dev
        <Directory "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/nad/">
                Options Indexes FollowSymLinks Includes ExecCGI
                AllowOverride All
                Order allow,deny
                Allow from all
                                Require all granted
        </Directory>
</VirtualHost>

<VirtualHost *:80>
    ServerAdmin razzaghi229@gmail.com
    DocumentRoot "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/api/"
        ServerName api.nad.dev
        <Directory "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/api/">
                Options Indexes FollowSymLinks Includes ExecCGI
                AllowOverride All
                Order allow,deny
                Allow from all
                                Require all granted
        </Directory>
</VirtualHost>

<VirtualHost *:80>
    ServerAdmin razzaghi229@gmail.com
    DocumentRoot "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/panel/"
        ServerName panel.nad.dev
        <Directory "/Users/shaghayegh/Projects/PHP/NADMultipleApp/web/panel/">
                Options Indexes FollowSymLinks Includes ExecCGI
                AllowOverride All
                Order allow,deny
                Allow from all
                                Require all granted
        </Directory>
</VirtualHost>


Remember when i want to add bundle correct default address