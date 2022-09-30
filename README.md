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

   Para ello desde nuestro equipo local hacemos un ping con la dirección de nuestra VB.

```
ping 10.28.2.100
```


   <img src="/img/Captura4-ping-desde-local.PNG" alt="imagen ipconfig" width="600px" />
