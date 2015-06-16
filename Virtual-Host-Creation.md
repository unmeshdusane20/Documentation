#Steps for creating Virtual Host in Windows

## Windows Platform 

1. Using XAMPP 

	1. Update the host file.
	 - You can find it under C:\WINDOWS\system32\drivers\etc\hosts(Open this file in Admin mode)
	 - At the end of file or next line after 127.0.0.1 localhost add 127.0.0.1 your-virtualhost-name(e.g- local.mysite.com)

	2. Update the vhost file in Apache configuration - 
	 - In XAMPP folder , open apache/conf/extra/httpd-vhost.conf file .
	 - Uncomment line #NameVirtualHost *:80 (line no 19-20) if it is commented.
	 - Add follwing code at the end of file.
	   ```<VirtualHost *:80>
    		DocumentRoot "path of your project root folder"
    		ServerName local.mysite.com
    		ServerAlias local.mysite.com    		
    		<Directory "path of your project root folder">
        		AllowOverride All
        		Order allow,deny
        		Allow From All
        		Options Indexes FollowSymLinks
    		</Directory>
		</VirtualHost>```
	 - Note : Order allow, deny
	          Allow From All
	          is used to access directory outside of the web root 
	          	
	3. Restart Apache.	
 	



