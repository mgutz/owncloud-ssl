# owncloud-ssl

Installs [owncloud](http://owncloud.org), an open source DropBox clone, onto
a Debian server with SSL certificate.

## Motivation

This is my data. There are many like it, but this one is mine! ... Without
my data, I am useless.

I use a $7/mo 250GB, 256M RAM storage plan from [BuyVM](buyvm.net) running Debian 6.06.

## How To

BEWARE the current version of ownCloud server is tweaking server-side encryption.
The next version promises to be better. Server-side encryption is not enabled
at this time.

Edit IP_ADDR and HOST_NAME variables in `install-owncloud-server`, then
from local terminal

    cat install-owncloud-server | ssh root@IP_ADDR /bin/bash

which runs `install-owncloud-server` script on your remote server.
