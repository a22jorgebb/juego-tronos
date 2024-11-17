## 0- Como todas las tareas se entregaron a las 23:59 no me dí cuenta que esta acababa por la mañana, por eso la entrego tarde.

## 1- Configuración dos ambitos e rangos de enderezos

- Rango de direcciones:

Ámbito red 192.168.11.0 - stark.lan

![](./images1/2024-11-16-23-22-44.png)
 
 Ámbito red 192.168.12.0 - lanister.lan  
   
![](./images1/2024-11-16-23-22-57.png)

- Reserva en ámbito 192.168.12.0 lanister.lan (cercei)

![](./images1/2024-11-16-23-23-07.png)


## 2- Configuración de opcións

Opciones red 11 stark

![images2](./images2/2024-11-16-22-35-13.png)

Opciones red 12 lanister

![images2](./images2/2024-11-16-22-35-19.png)


## 3- Configuración da actualización

Actualizaciones dns en ambos ámbitos DHCP (servidor tyrion, 2 interfaces y ámbitos)

![images3](./images3/2024-11-16-22-34-21.png)

Actualización DNS en el servidor tiwin red 12 - lanister

![images3](./images3/2024-11-16-22-41-47.png)

Actualización DNS en el servidor ayra reg 11 - stark

![images3](./images3/2024-11-16-22-51-37.png)


## 4- Vídeo no que o cliente renova a concesión, e se ve a zona DNS unha vez que o DHCP actualiza o DNS. Tamén o cliente debe ser capaz de resolver o seu propio nome (non FQDN).

- Vídeo de la renovación DNS y resolución propio nombre (no FQDN)

## [Enlace al vídeo](https://youtu.be/fzB_co86qUQ)


## 5- Clientes das dúas subredes, amosando DNS, router e enderezo IP.


- **Subred lanister.lan - 192.168.12.0**

Clientes

![images5](./images5/2024-11-17-16-12-28.png)


- Servidor DHCP
![images5](./images5/2024-11-17-16-13-45.png)



- **Subred stark.lan - 192.168.11.0**

Clientes

![images5](./images5/2024-11-17-16-14-09.png)

- Servidor DHCP

![images5](./images5/2024-11-17-16-15-57.png)


## 6- Configuración dos servidores failover.


![images6](./images6/2024-11-16-22-39-58.png)

## 7-Capturas dos clientes obtendo enderezos cos dous servidores failover encendidos, e con un acendido e outro apagado (de forma alterna)


![images7](./images7/2024-11-17-00-51-25.png)

![images7](./images7/2024-11-17-00-53-02.png)



## Elimina a interface de rede 192.168.11.8 de tyrion, e configura o servizo DHCP Relay no router. Comproba que os equipos da rede stark.lan reciben a configuración de rede de xeito correcto. Inclúe as capturas necesarias.


