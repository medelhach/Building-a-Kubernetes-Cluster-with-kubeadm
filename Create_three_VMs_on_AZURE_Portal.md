# Create virtual machines
* I create three VMs on azure portal and this is the VM configuration 
De base
```
Abonnement   :    P1-Real Hands-On Labs
Groupe de ressources -----------
Nom de la machine virtuelle   :    nodevm2kub
Région   :    West US
Options de disponibilité   :    Aucune redondance d'infrastructure requise
Type de sécurité   :    Standard
Image   :    Ubuntu Server 20.04 LTS - Génération 2
Taille   :    Standard D2s v3 (2 processeurs virtuels, 8 Gio de mémoire)
Type d'authentification   :    Clé publique SSH
Nom d’utilisateur   :    azureuser
Nom de la paire de clés   :    nodevm2kub_key
Ports d'entrée publics   :    SSH
Spot Azure   :    Non
```
* Disques
```
Type de disque de système d'exploitation   :    SSD Premium LRS
Utiliser des disques managés   :    Oui
Supprimer le disque de système d’exploitation avec la machine virtuelle   :    Activé
Disque de système d'exploitation éphémère   :    Non
```
* Mise en réseau 
``` 
Réseau virtuel   :    ----vnet
Sous-réseau   :    default (10.0.0.0/24)
Adresse IP publique   :    nodevm2kub-ip (nouveau)
Mise en réseau accélérée   :    Activé
Placer cette machine virtuelle derrière une solution d'équilibrage de charge existante ?   :    Non
Supprimer l’adresse IP publique et la carte réseau lors de la suppression de la machine virtuelle   :    Désactivé
```
* Administration   
```
Microsoft Defender pour le cloud   :    Aucun
Diagnostics de démarrage   :    Activé
Activer le diagnostic du système d'exploitation invité   :    Désactivé
Identité managée affectée par le système   :    Désactivé
Se connecter à Azure AD   :    Désactivé
Arrêt automatique   :    Désactivé
Activer hotpatch   :    Désactivé
Options d'orchestration de patch   :    Valeur par défaut de l'image
```
* Paramètres avancés
```
Extensions   :    Aucun
Applications de machine virtuelle   :    Aucun
Cloud init   :    Non
Données utilisateur   :    Non
Groupe de placement de proximité   :    Aucun
Groupe de réservations de capacité   :    Aucun
```
