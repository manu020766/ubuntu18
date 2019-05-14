# ubuntu18

## Instalar

* Node: https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04
* How to Install Visual Studio Code on Ubuntu 18.04: https://linuxize.com/post/how-to-install-visual-studio-code-on-ubuntu-18-04/
* Instalar Git:  sudo apt install git
* Instalar Vue: npm install -g @vue/cli
* Instalar LAMP: https://www.linode.com/docs/web-servers/lamp/install-lamp-stack-on-ubuntu-18-04/
* Instalar nvm, para poder activar diferentes versiones de node:
```
1- Si no tienes instalado curl: sudo apt-get install curl
2- Si ya tienes instalado node (lo desinstalamos): sudo apt purge nodejs npm
3- curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash   
4- Cerrar el terminal
5- Instalar node (último): nvm install node
6- To update node later on just do: nvm install node
                                    nvm alias default node
comandos habitulaes de nvm

nvm ls ----------------> Muestra las versiones de node instaladas en el sistema
nvm ls-remote --lts ---> Nos da un listado de las versiones de Node lts
nvm install v8.11.1 ---> Instala una version especifica y la activa
nvm use v12.2.0 -------> Selecciona la version de node que se utiliza
nvm uninstall v8.11.1 -> Desistala la version de node especificada


 
mas info: https://medium.com/devschile/m%C3%BAltiples-versiones-de-node-con-nvm-63b2ac715c38
```

## Errores trabajando con Visual studio code

```
"Visual Studio Code is unable to watch for file changes in this large workspace" (error ENOSPC)
When you see this notification, it indicates that the VS Code file watcher is running out of handles because the workspace is large and contains many files. The current limit can be viewed by running:

cat /proc/sys/fs/inotify/max_user_watches
The limit can be increased to its maximum by editing /etc/sysctl.conf and adding this line to the end of the file:

fs.inotify.max_user_watches=524288
The new value can then be loaded in by running sudo sysctl -p.
```

## Comandos Básicos

* reiniciar apache: sudo systemctl restart apache2
* paquetes instalados: dpkg --get-selections


## Permisos y propiedad de carpetas

* Permisos y Propiedad de carpetas/ficheros: http://www.lucid-lynx.com/?p=142

## Iniciar git

* Configuracion inicial git: https://git-scm.com/book/es/v1/Empezando-Configurando-Git-por-primera-vez

## Vue
### Linters

* ESlint rules essential Vue.js rules: https://eslint.vuejs.org/
* aribnb: https://github.com/airbnb/javascript
* standard: https://github.com/standard/standard
* prettier: https://prettier.io

