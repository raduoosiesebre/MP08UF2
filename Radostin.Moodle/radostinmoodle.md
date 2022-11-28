# Activitat Moodle v.4.5 | Instalació i Configuració

## Veurem com instalar Moodle i configurar-lo en un Ubuntu Server.
****

# Instalació: 

1: Actualitzarem els paquets abans de fer tot

![](assets/Selection_109.png)

2: Després instalarem apache2 amb aquesta comanda

![](assets/Selection_110.png)

3: Una vegada hem fet tot això, instalarém MariaDB <3

![](assets/Selection_114.png)

4: Després posarem aquesta comanda per configurar mysql

![](assets/Selection_115.png)

5: Posarem els paràmetres així

![](assets/Selection_116.png)
![](assets/Selection_117.png)

6: Una vegada hem configurat MySQL, afegirem el repositori per descarregar PHP

![](assets/Selection_118.png)

7:  Actulitzarem els paquets

![](assets/Selection_119.png)

8: Farem utilitzar aquesta comanda per instalar php7.3

![](assets/Selection_120.png)

9: Després descarreguem el fitxer zip de moodle amb la següent comanda:

``` wget https://download.moodle.org/download.php/direct/stable400/moodle-latest-400.zip ```

![](assets/Selection_121.png)

10:  Una vegada ho hem descarregat, instalarem unzip i descomprimirem el fitxer .zip al directori de apache2

```sudo apt install unzip```

```unzip (paquet.zip)```
![](assets/Selection_122.png)

11: Una vegada descomprimit ficarem permisos publics al directori de moodle

![](assets/Selection_123.png)

12: Entrarem a la carpeta home i farem una nova carpeta especial per moodle. Després li posarem permisos per al public també.

![](assets/Selection_124.png)

13: Una vegada hem fet tot això, entrarem a MariaDB amb aquesta comanda

![](assets/Selection_126.png)

14: Ficarem un nou usuari amb una contrasenya managermoodle

![](assets/Selection_127.png)

15: Després crearem la base de dades. 

![](assets/Selection_128.png)

16: Ficarem permisos al usuari que hem creat a la base de dades

![](assets/Selection_129.png)

17: Finalment posarem aquesta comanda i surti,

![](assets/Selection_130.png)

18: Una vegada hem fet tot estos passos correctament, per comprovar que hem fet tot bé, entrarem amb la adreça IP de la màquina o localhost/moodle.

![](assets/Selection_131.png)


