# Identifiant pérenne pour Topo.art
Document de travail pour documenter et planifier la **version 1** de l'identifiant unique pour les données de topo.art.

# Nomenclature
version `1.0`

# Changements :
- On sépare l'accès à la donnée de son identifiant unique.
- Ajout d'une uri pour l

# Racine de l'identifiant pérenne :
`http://topo.art/r/`
# Structure de l'identifiant
`^t[1-9][0-9]*$` (`tℕ`)

`ℕ` qui ne peux pas commencer par `0`

`ℕ` = nombre naturel.

`entité` = les types d'entités supportés dans Topo.art

## Les types d'entités
- Oeuvre
- Artiste
- Lieux
- Événement
- Organisation

## Longueur du nombre naturel `ℕ`
Mais les identifiants n'ont pas de limite de longueur, sauf celle technique pour gérer une base de données de cette grosseur :
- `http://topo.art/r/t1`
- `http://topo.art/r/t99999`
- `http://topo.art/r/t98123891876897162387951`

# Points d'entrés additionnels *(endpoints)*

## Accéder au json directement
`http://topo.art/r/[identifiant de l'entité]`.
Redirige directement du serveur avec une redirection `303`. Qui renvoie toutes les entités accessibles grâce au croisillon.
- `https://topo.art/uid/ldjson?uid=http://topo.art/r/uids/?[identifiant]`


## Voir le schema lorsque l'on travaille
- `https://topo.art/uid/preview?uid=http://topo.art/r/uids/?[identifiant]`


# Bibliographie
https://culturecreates.github.io/artsdata-data-model/id-and-uri-guidelines.fr.html
https://www.w3.org/TR/cooluris/#linking