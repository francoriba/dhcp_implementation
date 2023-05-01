# DHCP Server 

## ISC DHCP server (Deprecated)

Comandos: <br>
    ```sudo apt install isc-dhcp-server```<br>
    ```cd /etc/default```<br>
    ``` isc-dhcp-server ```<br>
    ```sudo cp isc-dhcp-server isc-dhcp-server.bak```<br>
   ```sudo nano isc-dhcp-server```<br>
    ```cd /etc/dhcp```<br>
    ```sudo cp dhcp.conf isc-dhcp.conf.bak```<br>

La interfaz de red configurada para ofrecer direcciones IPv4 e IPv6 es "ens192". Esto significa que el servidor DHCP sólo atenderá las solicitudes DHCP recibidas en la interfaz de red "ens192". Se puede verificar las interfaces disponibles con el comando ```ip addr ```.

## Kea DHCP server