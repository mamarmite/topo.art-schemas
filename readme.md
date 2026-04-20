# Dépôt des schémas de données structurées de Topo.art

Ces schémas de données stucturées ont été préparés pour TOPO – Centre de création numérique, dans le cadre du projet « Guide de gestion d'archives et de documents en arts numériques » afin de servir de gabarit pour le déploiement de données structurées sur les événements en arts visuels. Les schémas ont été développés par Dessa Hayes et Frédéric Julien, de CAPACOA. Ils ont été mis à disposition dans ce dépôt par Marc-André Martin afin de documenter et de partager les fruits du projet.

Pour les fins du projet de TOPO, nous avons un défini un schéma plafond pour les types entités suivantes:

- [Artiste](artiste.md)
- [Œuvre](oeuvre.md)
- [Événement](evenement.md)
- [Lieux](lieu.md)
- [Organisation](organisation.md)

Chaque lien renvoit vers un exemple de données structurées détaillées au format JSON-LD pour le type d'entité en question. Il s'agit de schémas plafonds : chaque exemple illustre toute la gamme des propriétés disponibles pour le type d'entités selon le vocabulaire Schema.org et le modèle de données d'Artsdata. Les organismes souhaitant déployer des données stucturées sur leur site pourraient choisir d'adopter des schémas simplifiés. Pour connaître les propriétés minimales requises pour chaque type d'entité, veuillez vous référer à la [documentation d'Artsdata](https://docs.artsdata.ca/index.fr.html).

# Identifiant pérenne

En plus des schémas de métadonnées descriptives, le projet a aussi définit stratégie de production et de publication d'[identifiants pérennes](https://www.artsdata.ca/fr/ressources/bien-identifie). Ces identifiants désignent de façon univoque chaque artiste, œuvre, événement, lieu et organisme dans le site topo.art. Les identifiants pérennes sont destinés à être renseignés sous la propriété `@id` dans les données structurées schema.org, conformément aux [recommandations d'Artsdata à propos des identifants pérennes](https://docs.artsdata.ca/identifiers-guidelines/identifier-recommendations.fr.html). 

Voici le document de travail de la version 1 de l'identifiant pérenne pour les données de topo.art :

[Identifiant pérenne](identifiant-unique.md)

# Notes

Quelques questions ont été posé et répondu pendant le projet. Quelques-unes ont été regrouper dans la section [Questions](questions.md)