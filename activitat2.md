## OwnCloud.

Primer tenim que començar explicant que es OwnCloud:

Owncloud és un servei d'emmagatzematge i sincronització de fitxers multiplataforma que es pot instal·lar al nostre servidor.
Amb ell, qualsevol usuari amb un compte pot pujar informació i se sincronitzarà amb els altres usuaris a qualsevol dels seus dispositius.

## Instalació OwnCloud.

Primer de tot tenim que instalar lo servidor apache amb les seguents comanes:

sudo apt install apache2

Instalem MariaDB:

![](algo.png)

I configurem MariaDB

sudo mysql_secure_installation

Deshabilitar usuarios anónimos.
Deshabilitar acceso remoto como root.
Eliminar las bases de datos de testeo y el acceso a las mismas.
Actualizar las tablas de privilegios.



