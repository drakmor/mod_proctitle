mod_proctitle
=============

Port of mod_proctitle to Apache 2.x.x

The code for Apache1 can be found at http://dammit.lt 

mod_proctitle.c -- Apache sample proctitle module

To play with this module first compile it into a DSO file 
and install it into Apache's modules directory by running:

    $ apxs -c -i mod_proctitle.c

Then activate it in Apache's httpd.conf file for instance
for the URL /proctitle in as follows:

    #   httpd.conf
    LoadModule proctitle_module modules/mod_proctitle.so

Then after restarting Apache via
    $ apachectl restart
