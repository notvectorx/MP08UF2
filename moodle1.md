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

Si tenim el segúent fallo tenim que instal·lar les extencions de php zip i curl.

![image](https://user-images.githubusercontent.com/114423166/205680737-2c815ce9-a1bf-4f0c-bf66-4b7c386dcb59.png)

![image](https://user-images.githubusercontent.com/114423166/205680778-3f4d3f29-91e5-46c1-af84-fb92dda805a3.png)

![image](https://user-images.githubusercontent.com/114423166/205680815-efa3ab36-122b-4f7f-b963-e1b9765e7e01.png)

I reiniciem lo Apache2
![image](https://user-images.githubusercontent.com/114423166/205681107-896c49e1-858d-40fa-80b4-8d6f6073815f.png)

I ja ens deixa entrar 

![image](https://user-images.githubusercontent.com/114423166/205681316-0ce75984-84bc-4373-aa22-a87c71ef64dd.png)

Posem la base de datos de MariaDB

![image](https://user-images.githubusercontent.com/114423166/205681444-ab2c3aa7-d08d-459a-ad35-2248885c714a.png)

Posem Usuari i Contrasenya:

![image](https://user-images.githubusercontent.com/114423166/205681579-c4fb54a7-4874-411a-8c7e-728d47fba16f.png)


Si ens surt lo següent error tenim que instal·lar  la extenció de php de mysql:

![image](https://user-images.githubusercontent.com/114423166/205681955-b0449eb0-0a27-4a1b-9410-9ec6052c7a21.png)

![image](https://user-images.githubusercontent.com/114423166/205682021-e34dc427-cc23-4df3-8cc0-cb07d1f3bd72.png)


despres instalem php8.0-xml i mbstring:

![image](https://user-images.githubusercontent.com/114423166/205682202-1ac944b5-1bfb-41c7-9198-6199b4ff0885.png)

![image](https://user-images.githubusercontent.com/114423166/205682323-8dd3b5c6-0238-4832-8751-571346773c22.png)

I reiniciem lo servidor Apache.

Ens surtiran els seguents errors que es soluciona instalant les extenciós de php que ens demanen:

![image](https://user-images.githubusercontent.com/114423166/205682585-356ee472-3a11-4978-8cbd-9428de7764ba.png)

Una vegada instalada les extencions podem continuar amb els seguents errors:

![image](https://user-images.githubusercontent.com/114423166/205683042-04ff884c-5386-4bf3-8a56-61fcef4519ad.png)


Tenim el seguent error que se soluciona en l'arxiu php.ini descomentant la següent linia i posant 5000:

![image](https://user-images.githubusercontent.com/114423166/205684583-9a90bbc8-0a2f-4f70-81ad-d86a3a251ae3.png)

![image](https://user-images.githubusercontent.com/114423166/205684645-877c3deb-430f-4390-add6-9655f008bd7b.png)
