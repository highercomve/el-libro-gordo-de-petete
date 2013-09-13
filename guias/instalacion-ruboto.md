Instalacion de Ruboto
====================

Ruboto es una gema de Ruby que nos permite programar para Android, haciendo uso del la JVM de Java sobre la implementacion de Ruby. Utilizando jRuby, por lo que tiene algunos requerimientos tecnicos.

## Requerimientos

- Java runtime y Java Compiler
- Android SDK
- jRuby y jruby-jars
- rvm
- En caso de tener el SO 64bits instalar ia32libs
- Apache ANT

Instalacion de Java

	sudo apt-get install openjdk-7-jdk

Instalacion de ia32libs (opcional)

	sudo aptitude install ia32-libs lib32ncurses5 lib32stdc++6

Instalacion de jRuby
	
	rvm install jruby-1.7.4
	rvm use jruby-1.7.4
	gem install jruby-jars

Instalacion de Apache ANT

	sudo apt-get -u install ant

Instalacion de Android SDK

Para instalar el sdk de Android solo es necesario descargarlo desde esta pagina [enlace](http://developer.android.com/sdk/index.html)

Luego de instalarlo extraerlo en el directorio de preferencia, en mi caso

	/home/sergio/android

Agregar $ANDROID_HOME a nuestras variables

	export ANDROID_HOME=/home/sergio/android

Agregar a el PATH las siguientes carpetas que estan dentro del SDK

	/tools/
	/plataform-tools
	/build-tools

El resultado podria ser algo asi:

	export PATH=$PATH:/home/sergio/Proyectos/android/sdk/tools:/home/sergio/Proyectos/android/sdk/build-tools:/home/sergio/Proyectos/android/sdk/platform-tools/ 

Instalacion de Ruboto

	gem install Ruboto
	ruboto setup



