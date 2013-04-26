Instalacion de Rails en Ubuntu
==============================

Instalacion de Ruby 1.9.3 y sus dependencias

    sudo apt-get install ruby1.9.1 libxml2-dev libxslt1-dev libsqlite3-dev gcc g++ libssl-dev libreadline6-dev zlib1g-dev linux-headers-generic curl git libmysqlclient-dev nodejs libmysql-ruby libcurl4-gnutls-dev libmysqld-dev ruby-dev ruby1.9.1-dev sqlite3 libmysql-ruby1.9.1 postgresql-client libpq-dev

Actualizacion del gem

    sudo REALLY_GEM_UPDATE_SYSTEM=1 
    gem update --system

Instalacion de Rails
  
    gem install rails

Instalacion de clientes de base de datos

    # PostgreSQL
    gem install pg

    # MySQL
    gem install mysql

> En caso de no tener servidores de Mysql, PHP, Phpmyadmin, etc. 
> Se puede instalar rapidamente el paquete tasksel para instalacion de Apache, PHP, Mysql

      sudo apt-get install tasksel
      sudo tasksel

      sudo apt-get install phpmyadmin
      sudo ln -s /usr/share/phpmyadmin /var/www/pma
