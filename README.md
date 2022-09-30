# P02-Instalar-Apache2

>By      **Bryan Jesús Rodríguez Ríos**   &middot;   **Alex Dario Masabanda Tituaña**

##  – Instalar Apache2 en una máquina virtual

Una vez importada la VirtualBox, arrancada y comprobado que tiene conexión a internet
Abrimos un terminal y procedemos a instalar y actualizar el sistema.

```
sudo apt-get update
sudo apt-get upgrade
```
 
   - [x] 1. Actualización sistema
   
   <img src="/img/Captura1-apt-get-update.PNG" alt="imagen campura1" width="600px" />

   - [x] 2. Upgrade

<img src="/img/Captura-upgrade.PNG" alt="imagen upgrade" width="600px" />

Con el sistema actualizado continuamos haciendo comprobaciones de red,
averiguando la ip del equipo local y de la máquina virtual

```
Local: CMD>ipconfig
VB: ifconfig
```

   - [x] 3. Comprobación red VirtualBox

   <img src="/img/Captura2-ifconfig.PNG" alt="imagen ifconfig" width="600px" />


   - [x] 4. Comprobación red equipo local

   <img src="/img/Captura3-ifconfig-local.PNG" alt="imagen ipconfig" width="600px" />

Una vez sabemos las direcciones de nuestros equipos procedemos a hacer un ping entre ellos.

   - [x] 5. Comprobación conexión entre equipos

   Para ello desde nuestro equipo local hacemos un ping con la dirección de nuestra VB y observamos que no hay perdida de datos.

```
ping 10.28.2.100
```


   <img src="/img/Captura4-ping-desde-local.PNG" alt="imagen ping" width="600px" />


###  – Como instalar Apache2 

Desde la terminal de la VB accedemos como super usuario.
```
sudo su
apt-get update
apt-get install apache2
```
Y realizamos un apt-get update.

   - [x] 6. apt-get update.

<img src="/img/paso1-installApache.PNG" alt="apt-get" width="600px" />

El siguiente paso es la instalación de apache2

   - [x] 7. Instalando apache2.

<img src="/img/paso2 install Apache2.PNG" alt="install apache" width="600px" />


Una vez ya instalado, podemos combrobar el estado de la instalación

```
apache2.service
```

- Algunos de los comandos de apache son:
```
service apache2 start  --> para arrancar
service apache2 stop  --> para pararlo
service apache2 restart --> reinicia ( equivalente a hacer stop y luego start )
service apache2 reload --> recargar la configuración
service apache2 status --> comprobamos el estado del servicio
```


   - [x] 8. Comprobando estado de apache.

Podemos ver que el estado esta **active**

<img src="/img/paso3 apache2 ejecutando.PNG" alt="apache active" width="600px" />


Para comprovar que apache se esta ejecutando, abrimos un navegador, ponemos ***localhost*** y nos aparece la paguina de apache.
Este fichero html se encuentra en la ruta /var/www/html

   - [x] 8. Página de apache.


<img src="/img/paso4 localhost.PNG" alt="localhost" width="600px" />


Accedemos al fichero index.html dirigiendonos a la ruta que hemos mencionado antes.

   - [x] 9. Index.html.


<img src="/img/paso5-index-html.PNG" alt="index" width="600px" />