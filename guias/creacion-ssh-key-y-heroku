Creacion de SSH Keys y configuracion de heroku
==============================================

Verificar que este creada la carpeta ~/.ssh

		ls ~/.ssh
		
		# En caso que no este creada
		mkdir ~/.ssh
		
Crear la clave SSH

		ssh-keygen -t rsa -C "correo@servidor.com"
		# Creates a new ssh key, using the provided email as a label
		Generating public/private rsa key pair.
		Enter file in which to save the key (/home/you/.ssh/id_rsa):

En caso de usar un pass para la clave publica no los solicitara 2 veces sino dejar en blanco

		Enter passphrase (empty for no passphrase): [Type a passphrase]
		Enter same passphrase again: [Type passphrase again]

Instalamos xclip para poder copiar la clave a nuestro portapapales de manera sencilla

		sudo apt-get install xclip

Y copiamos la clave para colocarla en github o donde sea necesaria.

		xclip -sel clip < ~/.ssh/id_rsa

## Manejar SSH Keys en heroku

Consultar todas las llaves:

		heroku keys

Para agregar una llave SSH en Heroku:
		
		heroku keys:add

Para eliminar una:

		heroku keys:remove correo@servidor.com


