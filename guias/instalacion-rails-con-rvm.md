Instalacion de rails con RVM
============================

## Instalacion de RVM

    sudo apt-get update
    sudo apt-get install curl
    
    \curl -L https://get.rvm.io | bash -s stable
    
    echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm"  # This loads RVM into a shell session.' >> ~/.bashrc

Reiniciar el terminal para que cargue el rvm

Comprobamos los requirimientos que solicita el rvm

    rvm requirements

Esto nos puede dar como resultado algo similiar a esto (en el caso de ubuntu)

    sudo apt-get install build-essential openssl libreadline6 libreadline6-dev git-core zlib1g zlib1g-dev libssl-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt-dev autoconf libc6-dev ncurses-dev automake libtool bison subversion pkg-config libxslt1-dev libsqlite3-dev gcc g++ libssl-dev zlib1g-dev linux-headers-generic git libmysql-ruby libcurl4-gnutls-dev libmysqld-dev ruby-dev ruby1.9.1-dev sqlite3 libmysql-ruby1.9.1 postgresql-client libpq-dev nodejs

## Instalacion Ruby

    rvm install 1.9.2
    rvm use 1.9.2 --default

Instalacion de manejador de gems

    rvm rubygems current

Instalacion de rails

    gem install rails