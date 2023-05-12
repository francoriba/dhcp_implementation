# DHCP Server

La funcion del servidor DHCP es la asignación automática de:<br>
* Direcciones IP
* Subnet Mask
* Default Gateway
* Servidor DNS

## ISC DHCP server (Deprecated)

Comandos: <br>
    ``` sudo su - ```<br>
    ``` apt install curl apt-transport-https -y ```<br>
    ``` curl -1sLf 'https://dl.cloudsmith.io/public/isc/kea-2-2/setup.deb.sh' | sudo -E bash ```<br>
    ``` apt install isc-kea-dhcp4-server -y  ```<br>
   ``` mv kea-dhcp4.conf kea-dhcp4.conf.bak```<br>
    ``` nano kea-dhcp4.conf ```<br>
   

La interfaz de red configurada para ofrecer direcciones IPv4 e IPv6 es "ens192". Esto significa que el servidor DHCP sólo atenderá las solicitudes DHCP recibidas en la interfaz de red "ens192". Se puede verificar las interfaces disponibles con el comando ```ip addr ```.

## Kea DHCP server
