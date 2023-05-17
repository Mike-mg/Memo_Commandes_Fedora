# Memo Commandes Fedora  
## Mise à niveau de Fédora  
1. Installation des plugins pour l'upgrade  
    `dnf install dnf-plugin-system-upgrade` 

2. Néttoyage du système  
    `dnf upgrade && dnf clean all`  

3. Upgrade du système  
    `dnf system-upgrade download --releasever=Numero_de_version < "Numero_de_version" est la nouvelle version à mettre à jour >`  

4. Redémarage du système pour l'upgrade et mise à jour  
    `dnf system-upgrade reboot`  
---
---
## DNF - Gestionnaire de paquet Fedora  
1. Mise à jour système et logiciels  
    `dnf update` ou `dnf upgrade`  

2. Vérification des mise à jour disponible  
    `dnf check-update`

3. Recherche de paquet  
`dnf search Nom_du_paquet` ou `dnf list nom_du_paquet`  

4. Information sur un paquet  
    `dnf info nom_du_paquet`  

5. Installation d'un paquet  
    `dnf install nom_du_paquet`
    
6. Installation de plusieurs paquets  
    `dnf install nom_du_paquet_1 nom_du_paquet_2 nom_du_paquet_3`  

7. Déinstaller un paquet  
    `dnf remove nom_du_paquet`  

6. Déinstaller plusieurs paquets  
    `dnf remove nom_du_paquet_1 nom_du_paquet_2 nom_du_paquet_3`  
---
---
## DNF - Utilisation des groupes  
1. Lister les groupes  
    `dnf grouplist`  

2. Informations sur les groupes  
    `dnf groupinfo "Nom_du_groupe"`  

3. Installation d'un groupe  
    `dnf groupinstall "Nom_du_groupe"`  

4. Désinstaller un groupe  
    `dnf groupremove "Nom_du_groupe"`  
---
---
## DNF - Néttoyage système  
1. Effacer le cache de dnf   
    `dnf clean dbcache`  

2. Effacer les paquets mis en cache lors du téléchargement  
    `dnf clean packages`  

3. Effacer tout les caches, les métadata et les fichiers inutiles de dnf   
    `dnf clean all`

4. Tout néttoyer en même temps  
    `dnf clean {dbcache,all,packages}`
