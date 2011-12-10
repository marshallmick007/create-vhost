# create-vhost

Simple script to help create apache virtual hosts for the
[MAMP](http://www.mamp.info) stack.

## Usage

    create-vhost sampledomain.tld

## Configuration

`APACHECONF` Set this to the path of your `httpd-vhosts.conf` file

`LOGDIR` Set this to the location you want apache logs

`VHOSTSDIR` Set this to the folder on your filesystem where you want new vhosts created


## What it does

1. Creates a new folder under the configured `VHOSTDIR` folder for your new
   virtual host
2. Adds an entry to your `/etc/hosts` file which will resolve the host
   name to your PC (Note: this requires `sudo`, so you will be prompted
for your password)

    127.0.0.1 sampledomain.tld
3. Appends a virtual host definition to your `httpd-vhosts.conf` file


