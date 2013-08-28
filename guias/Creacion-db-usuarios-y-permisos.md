Crear usuario de Base de datos Mysql con usuario y privilegios
==============================================================

Todos los comandos son ejecutados desde la consola de Mysql

	# Crear la base de datos
	create database nombre_de_basededatos;

	# Crear el usuario
	CREATE USER 'nombre_de_usuario'@'localhost' IDENTIFIED BY 'clave del usuario';

	# Dar permisos al usuario
	grant usage on *.* to nombre_de_usuario@localhost identified by 'clave del usuario';

	# Priviligios sobre la base de datos
	grant all privileges on nombre_de_basededatos.* to nombre_de_usuario@localhost ;

Migrar base de datos desde archivo .sql

	mysql nombre_de_basededatos < archivo_de_backup_sql.sql