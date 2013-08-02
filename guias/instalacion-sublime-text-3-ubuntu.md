Instalacion de Sublime-text 3 en Ubuntu
=======================================

Agregar los repositorios PPA webupd8team

	sudo add-apt-repository ppa:webupd8team/sublime-text-3
	sudo apt-get update

Instalar Sublime-text-3 (eliminara el sublime-text 2)

	sudo apt-get install sublime-text-installer

## Manejador de Paquetes

### Instalación del manejador de paquetes

Lo primero que hay que hacer es ir a la ruta donde el Sublime maneja los paquetes. En el caso de ubuntu es la siguiente:

	cd ~/.config/sublime-text-3/Packages

En caso de OS X debe ser algo parecido a esto:

	cd ~/Application\ Suport/Sublime\ Text\ 3/Packages

Ya dentro de la carpeta Packages procedemos a instalar el "Package Control"

	git clone https://github.com/wbond/sublime_package_control.git "Package Control"
	cd "Package Control"
	git checkout python3

### Instalar desde el manejador de paquetes los siguientes plugins.

El manejador de paquetes se utiliza presionando CTRL+SHIFT+P y buscando "package control: install", o desde Preferences -> Package Control

* Emmet
* Color Picker (ctrl + shitf + c)
* Placeholders
* Prefixr
* Tag (ctrl + alt+f )   para ordenar los html
* Alignment (ctrl + alt+ a)
* All Autocomplete
* AutoFileName
* BracketHighlighter
* Terminal
* Markdown Preview
* Git
* View in Browser