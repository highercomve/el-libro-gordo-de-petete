Instalacion de Passanger en Apache2
===================================

## Instalar Ruby por medio de RVM

## Instalar gem de passanger

		gem install passanger

## Instalar el modulo de apache2
		
		passenger-install-apache2-module

## Configuracion de HOST

Suppose you have a Rails application in /somewhere. Add a virtual host to your
Apache configuration file and set its DocumentRoot to /somewhere/public:

   <VirtualHost *:80>
      ServerName www.yourhost.com
      # !!! Be sure to point DocumentRoot to 'public'!
      DocumentRoot /somewhere/public    
      <Directory /somewhere/public>
         # This relaxes Apache security settings.
         AllowOverride all
         # MultiViews must be turned off.
         Options -MultiViews
      </Directory>
   </VirtualHost>

And that's it! You may also want to check the Users Guide for security and
optimization tips, troubleshooting and other useful information:

  /usr/local/rvm/gems/ruby-2.0.0-p247/gems/passenger-4.0.10/doc/Users guide Apache.html

Enjoy Phusion Passenger, a product of Phusion (www.phusion.nl) :-)
https://www.phusionpassenger.com
