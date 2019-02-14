## Présentation

Site web de l'association « Les Itinerrances » organisant de l'événement « Les itinerrances des poissons rouges ».
L'association est basée à Valence dans la Drôme.

Le site est disponible à cette addresse : http://les-itinerrances-des-poissons-rouges.fr

Le site est construit avec le générateur de sites web statiques [Jekyll](https://jekyllrb.com/).

## Installation

Jekyll utilise le language de programmation Ruby. Pour l'installer vous pouvez suivre [cette documentation](https://www.ruby-lang.org/fr/documentation/installation/).

Lancer ensuite les commandes suivantes :

    gem install bundler
    bundle install

## Génération du site web statique

Pour accéder en local au site web (http://localhost:4000/) et faire des modifications, lancer la commande suivante :

    bundle exec jekyll serve -w
    
Pour genérer le site web avant déploiement, lancer la commande suivante :

    bundle exec rake:build
