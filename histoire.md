# HISTOIRE

1950s: communications point a point
    ==> reseau *centralise*

1960s: debut creation reseau pour l'armee = Arpanet
    ==> reseau *maille*

|   ==> protocole TCP/IP
|

1990s: langage & protocole HTML

Elements necessaires a la communication *(ex du telephone)* = 
    - emetteur
    - recepteur
    - support de transmission
    - intermediaire *(transfo de la parole en signaux electriques puis vice versa)*
        ==> encapsulation

    > encapsulation = routines permettant lecture & manipulation + masquage

Regroupement des recherches dans une norme : modele OSI (1981)
    > objectif : evolutive & interoperabilite

# MODELE OSI

Modele theorique. En realite, utilisation du modele TCP/IP

## Communication par couches

### Couche 1 : Physique
    > offrir support de transmission
    = hub (concentrateur)

### Couche 2 : Liaison des donnees
    > connecter les machines entre elles sur un reseau *local*
    > detecter erreurs de transmission
    = switch (commutateur)

### Couche 3 : Reseau
    > interconnecter les reseaux entre eux
    > fragmenter les paquets
    = routeur

### Couche 4 : Transport
    > gerer les connections applicatives
    > garantir connection

### Couche 5 : Session
    non utilisee par TCP/IP

### Couche 6 : Presentation
    non utilisee par TCP/IP

### Couche 7 : Application
   = proxy 


## Regles

1. Chaque couche est independante
2. Chaque couche ne peut communiquer qu'avec une couche adjacente (= directement sous elle)


# COUCHE 2 : LIAISON DES DONNEES

Connecter des machines sur un reseau local

## L'adresse MAC

### Notation

Codee sur 6 octets = 48 bits
    > 1 octet = 8 bits = 2^8 valeurs = 256 valeurs


