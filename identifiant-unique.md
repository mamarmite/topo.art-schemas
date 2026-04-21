# Identifiant pérenne pour Topo.art
Document de travail pour documenter et planifier la version 1 de l'identifiant unique pour les données de topo.art.
# Nomenclature
version `0.8`

En cours de travail : version `0.9` , on y va avec un identifiant sans type dans le nom et avec une redirection 303 pour le json+ld.

# Changements :
- organisation est maintenant avec un identifiant interne aussi.
- On utilise le croisillon pour les identifiants.
- On sépare l'accès à la donnée de son identifiant unique.
# Racine de l'identifiant pérenne :
`topo.art/r`
# Structure de l'identifiant
`^[aepco][1-9][0-9]*$` 
(`[entité][NNNNNNN]`)

`N` qui ne peux pas commencer par `0`)
`N` = nombre naturel.
`entité` = les types d'entités supportés dans Topo.art
## Les types d'entités
- Oeuvre (*`C`reative work*)
- Artiste (*`A`gent*)
- Lieux (*`P`lace*)
- Événement (*`E`vent*)
- Organisation (*`O`rganisation*)
### Oeuvre (`c`)
`topo.art/r#cNNNNNNN
`c` pour `creativeWork`
### Artiste (`a`)
`topo.art/r#aNNNNNNN`
`a` pour `artiste` et `agent`
### Lieux (`p`)
`topo.art/r#pNNNNNNN`
`p` pour `place`
### Événements (`e`)
`topo.art/r#eNNNNNNN`
`e` pour `event`
### Organisation (`o`)
`topo.art/r#oNNNNNNN`
`o` pour `organisation`
## Longueur du nombre naturel
J'ai mis 7x `N` dans l'identifiant unique.
Mais les identifiants n'ont pas de limite de longueur :
- `topo.art/r#a1`
- `topo.art/r#e99999`
- `topo.art/r#p98123891876897162387951`

# Points d'entrés additionnels *(endpoints)*

## base pour
`topo.art/r`.
Qui renvoie toutes les entités accessibles grâce au croisillon.

**Proposition comme endpoint** :
- `topo.art/r/uids/?[identifiant]`
Qui renvoie la donnée en format `json+ld` par défaut.

- `topo.art/r/view/[identifiant]` Qui renvoie à une page qui permet à un humain de le lire le json+ld sans devoir ouvrir le code source de la page.

# Bibliographie
https://culturecreates.github.io/artsdata-data-model/id-and-uri-guidelines.fr.html
https://www.w3.org/TR/cooluris/#linking