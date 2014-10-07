Instalacion PostgreSQL Ubuntu
=============================

1.- Instalar postgre y el admin tool desde el manejador de paquetes

    sudo apt-get install postgresql libpq-dev phppgadmin pgadmin3

2.- Configurando postgre

    sudo nano /etc/postgresql/9.1/main/postgresql.conf

Descomentar #listen_addresses = localhost
Descomentar #password_encryption = on

Salvar el archivo y reiniciar

    sudo service postgresql restart

3.- Crear un usuario para postgre

    sudo -u postgres createuser -P -s -e <nuevo_usuario>
