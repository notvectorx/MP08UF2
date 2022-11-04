Bones estimat/ada treballador,

Enviem aquest mail perque la nostra empresa a implementat un gestor d'arxius online completamenmt nou i en aquest e-mail
li explicarem pas a pas com s'instala aquest nou programa amb lo nom i contrasenya d'usuari que posarem a la vostra dispocició
en aquest nou gestor d'arxius disposara de 600MB d'almacenatge.

NOM USUARI: "owncloud-client1"

CONTRASENYA: "SBc(UtRwl"

### INSTRUCCIONS INSTALACIÓ OWNCLOUD

#### Sistema Operatiu LINUX UBUNTU

Amb aquestes comandes podrem instalar lo client de owncloud per a poder conectarnos al servidor.


`wget -nv https://download.owncloud.com/desktop/ownCloud/stable/latest/linux/Ubuntu_22.10/Release.key -O - | sudo apt-key add -`

`echo 'deb https://download.owncloud.com/desktop/ownCloud/stable/latest/linux/Ubuntu_22.10/ /' | sudo tee -a /etc/apt/sources.list.d/owncloud.list`

`sudo apt update`

`sudo apt install owncloud-client`






