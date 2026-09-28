# RentIT

![Cas d'utilisation RentIT](01.svg)

---
 
# Inscription d’un membre (OCEANE)

## Cas d’utilisation #1

## Objectif à atteindre

Le **membre** saisit ses renseignements personnels afin de créer un compte dans l’application **RentIT**.

## Acteurs

### Acteur principal

- **Membre**

### Acteurs secondaires

- **Application RentIT**
- **Serveur**
- **Base de données**

## Parties prenantes et intérêts

- **Membre** : souhaite créer un compte  afin de pouvoir utiliser les services de location.
- **RentIT** : souhaite conserver des renseignements valides sur les membres inscrits.
- **Serveur** : valide les informations saisies avant de les enregistrer.
- **Base de données** : conserve les informations du membre de manière sécurisée.

## Description

Le membre remplit un formulaire d’inscription avec ses informations personnelles. Le serveur valide les informations saisies. Si les informations sont valides, elles sont enregistrées dans la base de données et l’inscription est confirmée.

## Préconditions

- Le membre s'est authentifié 


## Scénario nominal

1. Le **membre** accède au formulaire d’inscription.
2. Le **membre** saisit son nom.
3. Le **membre** saisit son numéro de téléphone.
4. Le **membre** saisit son adresse de domicile.
5. Le **membre** saisit sa date de naissance.
6. Le **membre** soumet le formulaire d’inscription.
7. L’**application RentIT** envoie les informations au **serveur**.
8. Le **serveur** valide le format des informations saisies.
9. Le **serveur** enregistre les informations du membre dans la **base de données**.
10. L’**application RentIT** affiche le message : « Inscription terminée ».
11. Le membre peut maintenant utiliser son compte RentIT.

## Scénarios alternatifs

### A1 — Informations invalides

1. Le **serveur** détecte qu’une ou plusieurs informations sont invalides ou incomplètes.
2. L’**application RentIT** affiche le message : « Veuillez mieux remplir le formulaire ».
3. Le **membre** corrige les informations demandées.
4. Retour à l’étape 2 du scénario nominal.

## Postconditions

- Un compte membre est créé dans l’application **RentIT**.
- Les informations personnelles valides du membre sont enregistrées dans la base de données.
- Le membre peut se connecter à son compte.
- Si le membre a ajouté une carte de crédit valide, celle-ci est associée à son compte.
- Le membre peut ensuite effectuer une réservation de véhicule.

## Diagramme de séquence

![Diagramme de séquence — Inscription d’un membre](03.svg)

---

![Modèle du domaine RentIT](04.svg)

![Diagramme d'état d'un véhicule chez RentIT](05.svg)