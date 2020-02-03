#SubRedes
 Calculamos la mascara de sub red para cada una de las subredes que hay en la red, para la primera sub la mascara sera 255.255.255.128, para la segunda sera 255,255,255,224 y para la tercera 255.255.255.248.


#Servidores DHCP

Para esto tendremos que hacer un servidor _DHCP_ el cual de direcciones automaticamente a cada usuario conectado, para ello iremos a la configuracion del servidor y le daremos una ip y una mascara, por defecto, junto a esto le daremos un gateway por defecto y un servidor _DNS_, en los servicios del servidor activaremos el _DHCP_ junto a ello le daremos la gateway que pusimos anteriormente y el servidor _DNS_ y una ip de inicio con la cual comenzara a dar ip a partir de ella a cada usuario conectado hasta el numero maximo de ususarios que le asignemos, tambien dara una mascara por defecto
Este servidor tambien almacena los puntos de acceso a los servidores web mediante el servicio de DNS, solo hay que añadir las ip dentro del servicio _DNS_. 
Con esto ultimo tambien habremos activado el servicio de servidor WEB.


#Routers
    Para el primer _Router_ y para los siguiente lo primero que haremos sera apagarlo para añadirle varios modulos necesario para poder unir la redes, añadiremos el modulo HCWIT-2  a la derecha y el WIC-2T a la izquierda, con esto volvemos a enceder el router y vamos a Config.
    Vamos al FastEthernet al cual esta conectada la red y le damos la ip del router en la red y una submascara, por defecto. Continuamos configurando el _SERIAL_, para ellos vamos a un serial cualquiera y añadimos un ip propia del router y una mas cara de subred y un rango. 
    Para finalizar vamos a _RIP_ y añadimos la ip propia del router y la ip que tiene el router dentro del servidor.
    Para la configuracion de los siguientes routers añadiremos en el _RIP_ la ip propia del router de delante, la ip del propio router dentro de la red y si la conexion de los routers no termina hay, es decir, hay otro router destras de este que estamos configurando, se añade la ip propia del router. 

    




