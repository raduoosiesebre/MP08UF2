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

18: Una vegada hem fet tot estos passos correctament, per comprovar que hem fet tot bé, entrarem amb la adreça IP de la màquina o localhost/moodle. Si ens funciona, seleccionarem un llenguatge i li donarem a següent

![](assets/Selection_131.png)

19: Ara ens diu que ens falta alguns paquets. Per tant els instalarem amb la següent comanda

```
sudo apt install php7.3-curl -y
sudo apt install php7.3-zip -y
```

![](assets/Selection_199.png)

20: Després reiniciarem el servidor web amb aquesta comanda
```
sudo service apache2 reload
```

21: Un cop ho tenim reiniciat vorem aquesta pantalla. Aquí hauriem de posar aquest directori al tercer camp

```
/home/moodledata
```

![](assets/Selection_204.png)

22: Un cop hem donat següent, hauriem de seleccionar la base de dades MariaDB

![](assets/Selection_205.png)

23: Després hauriem de emplenar els camps amb les dades que vam omplir cuan vam configurar la base de dades

![](assets/Selection_206.png)

24: Després instalarem els següents ordres

```
sudo apt install php7.3-mysql
sudo apt install php7.3-xml
sudo apt install php7.3-mbstring
sudo apt install php7.3-gd
sudo apt install php7.3-intl
sudo apt install php7.3-xmlrpc
sudo apt install php7.3-soap

sudo service apache2 restart
```

25: Després cuan tinguesim la pàgina reiniciada, veurem aquesta pantalla. Li donarem a continuar per aceptar els termes de condicio

![](assets/Selection_210.png)

26: Després ens apareixerà una altra finestra amb tots els continguts que els está verificant moodle per la instalació necessària

![](assets/Selection_215.png)

27: Una vegada hem fet continuar, es començara la instalació de moodle. Un cop finalitzada farem click en continuar

![](assets/Selection_216.png)
![](assets/Selection_217.png)


28: Aqui tenim que omplir dades com nom d'usuari, contrasenya, email, etc. Un cop hem acabat farem click en següent

![](assets/Selection_218.png)
![](assets/Selection_219.png)

29: Després posarem informació per el nostre moodle. Nom, Descripció, Zona horaria, etc.

![](assets/Selection_220.png)
![](assets/Selection_221.png)

30: Ja tenim el nostre moodle listo per utilitzar!

![](assets/Selection_222.png)
