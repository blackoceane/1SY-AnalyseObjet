
# _Retirer de l argent_

### Cas d'utilisation \#_001_

## Objectif à atteindre
Retirer de l'argent a un guichet automatique d'une institutions financières

## Acteurs

### Primaire
Utilisateur 
### Secondaires

navigateur
serveur 



## Parties prenantes et intérêts
AUCUN

## Description

### Précontidions

- il doit s authentifier 
- I reste des sous dans le guichet 


### Scénario nominal

_Inscrire de façon numérotée, chacune des interactions entre les différents participants du système. Considérer ici le scénario nominal (avec vos lunettes roses, quand tout va pour le mieux). Utiliser le mode `ping-pong`_

2. l 'utilisateur selectionne retirer de l' argent 
3. l utilisateur entre la somme d argent a retirer 
4. le navigateur renvoie la requete au serveur 
5. le serveur renvoie la requete au service d institution financiere 
6. le serveur renvoie la reponse la reponse a le navigateur
7.  si c est pas correct le navigateur  affiche refuser "pas assey de fond"   
8. si corect la machine sort de l' argent en espece


### Postconditions
l' argent sort de la machine 
