### Instal·lem Apache 2 amb la següent comana:

```
sudo apt install apache2
```

![Captura de pantalla de 2022-11-28 19-33-58](https://user-images.githubusercontent.com/114423166/204357146-8c0cb098-bfc5-4184-8045-a37ea23eade8.png)

### Instal·lem MariaDB 2 amb la següent comana:

```
sudo apt-get install mariadb-server
```
![image](https://user-images.githubusercontent.com/114423166/204357842-7890d66b-88de-46ca-a0c4-76e525e15e0c.png)

### Configurem les opcions de seguretat de mariaDB amb la següent comana:
```
sudo mysql_secure_installation
```
![image](https://user-images.githubusercontent.com/114423166/204358305-54fa072b-b764-4c7d-9fc2-3587fb59f27d.png)

### Instal·lem PHP

Per a instalar la versió de php que volem tenim que instalar primer un repositori que es fa amb la seguent comana:
```
sudo add-apt-repository ppa:ondrej/php
```

Una vegada instalat lo repositori podem instalar lo PHP en aquest casa la versió 8.0.
```
sudo apt install php8.0 libapache2-mod-php8.0
```
![image](https://user-images.githubusercontent.com/114423166/204359711-27b5721b-9159-4328-b572-d28980ba49e7.png)

Amb la comana "php-v" podem veure la versió de lo nostre php.
![image](https://user-images.githubusercontent.com/114423166/204359856-4be84e30-f035-435b-8be4-3cad9d9a62f3.png)

### Una vegada tenim instalat "LAMP" ja podem iniciar amb l'instalació del moodle.

Primer tenim que descaregar lo moodle amb la comana:
```
wget https://download.moodle.org/download.php/direct/stable401/moodle-4.1.zip

![image](https://user-images.githubusercontent.com/114423166/204360485-16d0638a-ac0d-4e1f-9409-8e976698a3ec.png)
```
![image](https://user-images.githubusercontent.com/114423166/204361033-d0dc3073-4c04-4d27-a750-a8f52dd46742.png)


Descomprimim l'arxiu amb la següent comana:
```
sudo unzip moodle-latest-38.zip -d /var/www/html/
```
Ara toca cambiar els permisos del directori:

![image](https://user-images.githubusercontent.com/114423166/204361991-1d9972a0-2d4e-4642-891e-be23bdfbe4b1.png)

Creem un dirrectori de fitxers:

![image](https://user-images.githubusercontent.com/114423166/204362116-a4b8d05d-2b03-4759-884d-d3bf4b46757b.png)


Configurem la Base de dades de MariaDB

![image](https://user-images.githubusercontent.com/114423166/204362740-2da588f9-bab0-4886-9e75-90f865eeef88.png)

Una vegada fet aixos podem iniciar desde un navegador per a iniciar amb la configuració de lo nostre moodle.

![image](https://user-images.githubusercontent.com/114423166/204363067-3fd76f8c-6960-450b-a589-af860a224779.png)





