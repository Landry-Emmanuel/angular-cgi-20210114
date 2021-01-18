*********************** PULSE ***********************
usr: CGI_VINOT
pwd: 0909		//Hellspawn0

usr: CGI_WETOUMDIE
pwd: 1994



*********************** GIT ***********************
usr: CGI_VINOT
pwd: Hellspawn0

usr: CGI_WETOUMDIE
pwd: uwe1k6Dw

[15:18] PRIOUL, Arnaud
    deja va falloir que tu change de compte dans ta config git
(1 mentions J'aime)​[15:19] PRIOUL, Arnaud
    ensuite tu va devoir generer une clef ssh sur ton ordi et config ton ssh pour que sur l'ur du git en question il prenne la bonne clef ssh
​[15:19] PRIOUL, Arnaud
    ensuite tu va devoir te connecter sur le gitlab et ajouter ta clef afin que gitlab sache bien que c'est toi qui push



*********************** AU REDEMARRAGE DU PC ***********************
Editer le registre windows (HKEY_LOCALMACHINE) avec :
Nom de la valeur: S2E_VPN_partcgi
Données de la valeur: Jbxajr63:/!b(C3H


*********************** SERVEUR NAOS ***********************
url : S2ENAOAPPC01R.orion.s2e-net.com
usr : adminomc
port : 22
pswd : HZHlsTNMH79IkAQO2p1c

--> Commandes de conexion au serveur de RECETTE :
	- sudo su tomcat-rec
	- cd /opt/rec/tomcat/logs/
	- tail -f catalina.out
	
--> Commandes de conexion au serveur de DEV :
	- sudo su tomcat-dev
	- cd /naos-dev/opt/tomcat/naosc01d/logs/
	- tail -f catalina.out
	
	*** Redémarrer le serveur :
		- sudo systemctl stop tomcat-dev
		- sudo systemctl start tomcat-dev
 


*********************** BDD NAOS ***********************
--> Dev, Int : mdp = vendredi

*********************** URL TEST S2E ***********************
url http://s2enaoappc01r:8080/naos/entreprise/entreprises
usr/mdp: 00005822




*********************** COMMANDES ANGULAR/NODE ******************************
Commande de configuration du proxy pour installer les commandes NPM et ANGULAR
(npm config list : pour vérifier les configs en place)

---> "npm config set proxy "http://proxy.global.logica.com:80"
---> "npm config set proxy-https "http://proxy.global.logica.com:80" 
---> "npm config set proxy_https "http://proxy.global.logica.com:80"

---> "npm install -g @angular/cli" : installe angular cli
---> "npm cache clean --force" : vide le cache npm

---> "ng serve" ou "npm start"(si le projet n'a pas été créé localement, mais a plutôt été récupérer sur un 
upport quelconque) : lance une application angular

---> Generating a spec file after generated the component :
"ng g component <your-component> --spec-only"




*********************** COMMANDES GIT ******************************
---> git branch <Nouvelle Branche> : créé une nouvelle branche
---> git push --set-upstream origin <Nouvelle Branche> : push la nouvelle branche sur le repertoire distant
---> git symbolic-ref HEAD --short : affiche le nom de la branche sur laquelle vous vous trouvez
