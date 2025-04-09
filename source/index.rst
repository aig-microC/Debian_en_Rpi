=====================================================
Instalación de *DEBIAN* nativo en una *Raspberry Pi*
=====================================================

Introducción
------------

En este documento se describe como instalar el *Sistema Operativo Debian* en una `Raspberry Pi`_. Esta tarjeta, que es un ordenador completo, tiene su propio sistema operativo oficial: *Raspberry Pi OS (de 32 o 64-bits)* que se puede obtener de https://www.raspberrypi.com/software/operating-systems/ y que es un derivado de *Debian* *estable*, optimizado para esta tarjeta. Yo prefiero trabajar con un sistema *Debian* nativo y en su versión *testing*, si ya la versión estable tiene más de 3 o 6 meses de antigüedad.

.. _`Raspberry Pi`: https://www.raspberrypi.com/

A continuación te muestro el procedimiento para realizar una instalación de *Debian* en una tarjeta *microSD* ya sea para la versión *estable* o la *testing*.

Básicamente, la selección de la imagen de partida (ver https://wiki.debian.org/RaspberryPi y la respuesta 6 de https://raspi.debian.net/faq/) depende de la *familia* a la que pertenece la tarjeta de la *Raspberry Pi*. 

-   Las *Raspberry Pi Zero*, *Raspberry Pi Zero W* o *Raspberry Pi Zero WH* utilizan un chip que se corresponde con una arquitectura de 32 bits de tipo *armel* lo que supone que no dispone de una unidad de coma (punto en inglés) flotante (*FPU* *Floating Point Unit*) para las operaciones de cálculo. Los cálculos los hace mediante software y por lo tanto es más lento que si dispusiera de una *FPU*. En la notación que utiliza *Debian* es de la **familia 0/1**. No consideraré la *Raspberry Pi Zero* porque no tiene conectividad con la que acceder a *Internet* mientras que las que si la tienen, *W* y *WH*, solo se diferencian en si tiene (*WH*) o no (*W*) la tira de de pines para conexiones (*GPIO*) soldada. A esta familia pertenecen también las *Raspberry Pi A, B, A+, B+ y las mencionadas Zero, Zero W*)

-   La *Raspberry Pi 2* tiene arquitectura *amrhf* de 32 bits con 1 GB de memoria *RAM*. En la notación que utiliza *Debian* es de la **familia 2**

-   La *Raspberry Pi Zero 2W* es de 64 bits con *FPU*. Su arquitectura es *armhf*. Tiene, como la *Zero W* 512 MB de memoria *RAM* por lo que si instalas un escritorio (sí, se puede instalar un escritorio y tener un entorno gráfico) no será muy rápido (pero un poco más rápida que si lo pruebas en una *Zero W*). En la notación que utiliza *Debian* es de la **familia 3**. A esta familia pertenecen también las *Raspberry Pi 3, 3A+, 3B+ y la mencionada Zero 2 W*).

-   Las *Raspberry Pi 4* y *Raspberry Pi 400* son las versiones más potentes, con arquitectura *arm64* de 64 bits y 4 GB de memoria. La *Raspberry Pi 4* dispone de una versión con 8 GB de memoria *RAM*. En la notación que utiliza *Debian* es de la **familia 4**.

Este documento está bajo  `Licencia Creative Commons Atribución-CompartirIgual 4.0 Internacional`_. Todas las marcas comerciales referidas en este documento pertenecen a sus legítimos propietarios.

.. figure:: imágenes/CC.png
   :scale: 25 %
   :align: center

..  _`Licencia Creative Commons Atribución-CompartirIgual 4.0 Internacional`: https://creativecommons.org/licenses/by-sa/4.0/

La última versión de este documento está en https://github.com/aig-microC/Debian-en-RaspberryPi.

.. raw:: latex

   \newpage

.. toctree::
   :maxdepth: 2
   :caption: Contenido:
   
   DebianNativoRPi.rst


