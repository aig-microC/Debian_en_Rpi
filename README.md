# Instalar Debian nativo en Raspberry Pi

## Guía o Tutorial para instalar Debian en una Raspberry pi 4 o 400

Como instalar el *Sistema Operativo Debian* en una `Raspberry pi 4 o 400`. Esta tarjeta, que es un ordenador completo, tiene su propio sistema operativo oficial: *Raspberry Pi OS (de 32 o 64-bits)* que se puede obtener de https://www.raspberrypi.com/software/operating-systems/ y que es un derivado de *Debian* *estable*, optimizado para esta tarjeta. Yo prefiero trabajar con un sistema *Debian* nativo y en su versión *testing*. Aquí podrás ver como se puede instalar la versión *estable* o la versión *en pruebas* o *testing*.

En esta versión se incluyen los ficheros fuentes para generar esta documentación con *SPHINX*. Los documentos finales son *debiannativoenunarpi.pdf* y en *HTML* los ficheros que están en el subdirectorio *html* (realmente son enlaces simbólicos a los correspondientes ficheros que estń en *build*).

Para clonar el repositorio (ihacer una copia local en tu PC) necesitas tener instalado *git*. Para ello, si no lo tienes instalado puedes hacerlo con:

_sudo apt install git_

y para clonar el reprositorio

_git clone https://github.com/aig-microC/Debian-en-RaspberryPi_


Para compilar y generar la documentacióni, en el subdirectorio donde ves losficheros  _Makefile_ y _README.md_ hay que teclear:

_make html_

para generar la version *html* o

_make latexpdf_

para la versión en *PDF*

Para ver los posibles tipos (formatos) de documentos que se pueden generar, simplemnte, teclear

_make_
