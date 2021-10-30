# apache2-guide

## Install Apache server:
Run the following command to install Apache.
    
    apt-get install apache2
Run the following command to start the Apache process.
    
    /etc/init.d/apache2 start
Verify that the service is running by executing the following command.
    
    /etc/init.d/apache2 status
Run the following command to restart Apache.
    
    /etc/init.d/apache2 restart
You can also check the status using the following command,
    
    sudo systemctl status apache2.service

## Configure Apache Server:
The next step is to set up the web server configuration for the domain. The Apache configuration directory is "**/etc/apache2**" and "**apache2.conf**" is main Apache configuration file. Each domain needs its own Virtual Host configuration file. Here you can configure apache server according to your requirements. But most cases we use the default configurations.
By default, apache will provide a root directory for our web services to be deployed which is "**/var/www/html**". this is configured as the root directory of apache server.
we can find a file called "index.html" in the root directory. after starting the apache service if we open any browser from our machine and enter the following url, 
  
    http://localhost
This will show the index.html file from the apache root directory.
Now lets say clone the web application from the git repository from [here](https://github.com/aminul-hq/apache2-guide.git). This is a simple web application for testing the deployment in apache server.
