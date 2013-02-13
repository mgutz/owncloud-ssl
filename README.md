# owncloud-ssl

Installs [owncloud](http://owncloud.org), an open source DropBox clone, onto
a Debian-based server with SSL certificate.

## Motivation

This is my data. There are many like it, but this one is mine! ... Without
my data, I am useless.

I use a $7/mo 250GB, 256M RAM storage plan from [BuyVM](http://buyvm.net) running Debian 6.06.

## How To

Log into your remote server

Download the script

    wget https://raw.github.com/mgutz/owncloud-ssl/master/install-owncloud-server

Edit IP_ADDR and HOST_NAME variables in `install-owncloud-server`

On Ubuntu (recommended with encrypted partition), 50MB RAM footprint

    sudo bash install-owncloud-server

Or Debian (as root), ~40MB RAM footprint

    bash install-owncloud-server


## Server Side Encryption

BEWARE, OwnCloud server side encryption is disabled because it is known to have issues
and is being addressed in the next major version.

My suggestion is to not deal with it and install ownCloud on Ubuntu Server 12.04 or
greater and use encrypted LVM partiation when installing the OS. Your entire
server data then is safe from prying eyes as they will only see gibberish
including file and directory names. Encryption comes with a huge performance cost
which is more than acceptable.

