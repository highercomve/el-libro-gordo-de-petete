Instalacion de Sublime-text en Ubuntu
=====================================

Agregar los repositorios PPA webupd8team

    sudo add-apt-repository ppa:webupd8team/sublime-text-2
    sudo apt-get update

Podemos instalar dos versiones de sublime, la version Beta o la version en desarrollo

    # Beta
    sudo apt-get install sublime-text-2-beta

    # Desarrollo
    sudo apt-get install sublime-text-2-dev
    
Instalacion de paquetes.

1.- Instalar el manejador de paquetes

ir a “view/console view” y pegar esta línea y presionar enter

    import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'
    
2.- Instalar desde el manejador de paquetes los siguientes plugins.

El manejador de paquetes se utiliza presionando CTRL+SHIFT+P y buscando "package control: install"

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

