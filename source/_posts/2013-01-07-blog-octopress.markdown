---
layout: post
title: "Contribuer au blog JCertif Lab"
date: 2013-01-07 22:59
comments: true
categories: octopress, blog
author: Rossi Oddet
---
Ce blog est construit autour du produit [Octopress](http://octopress.org/).

## Pourquoi Octopress ?
Plusieurs outils de génération de blog existent : Blogger, Wordpress, Google Site etc... Ces outils ont un point commun : la rédaction d'article en ligne.

Dans notre contexte africain où certaines régions sont encore mal desservies, être dépendant d'une connexion internet durant la phase de rédaction représente un inconvénient majeur. 

Un contributeur doit pouvoir rédiger librement son article avec toutes ses ressources en local (sur son poste) et mettre à disposition son travail par le biais d'une synchronisation.

C'est précisement sur ce mode d'utilisation que Octopress, Git et Github vont se révéler très pratique.

#### L'édition d'article se fait en markdown
Ecrire un article revient à écrire dans un fichier texte sans se soucier de la mise en forme. C'est comme si vous écriviez le brouillon d'un article avec un notepad et que ça suffisait pour l'avoir en ligne :)

Le contributeur peut écrire son article avec l'éditeur texte de son choix (Notepad, Vi, Sublime Text, ...).

Sauvegarder les articles sans mise en forme est un bon moyen de stockage des articles et facilite les futurs migrations vers d'autres moteurs de blog.

#### Git est offline !
Git est un gestionnaire de version de fichiers, un peu comme SVN, avec une grande différence : il fonctionne en mode offline.

Avec Git, on gère l'historisation de nos fichiers, les branches, ... en local et on utilise le réseau internet que pour se synchroniser avec d'autres dépôts.

Le contributeur peut ainsi gérer ses modifications, faire des retours arrières etc... sans avoir besoin du réseau internet. Il n'utilise internet qu'au moment de partager à d'autres ses articles.

#### Le blog généré par Octopress est statique
Ce qui rend la recherche d'hébergeur très aisé. Il nous est donc possible de l'héberger gratuitement sur Github sans avoir à effectuer la maintenance d'un serveur web.

#### Octopress est extensible
Il y a de nombreux [plugins](https://github.com/imathis/octopress/wiki/3rd-party-plugins) et il est très simple d'en créer pour des besoins spécifiques.

## Comment contribuer ?

####	Pré-requis

*	Avoir un compte [Github](http://www.github.com)
*	[Git](http://git-scm.com/book/en/Getting-Started-Installing-Git) est installé. 

####	Récupérer les sources depuis Github
{% gist 4532971 %}

####	Créer un fichier dans le répertoire source/_posts

Le fichier doit s'appeler [YYYY-MM-DD-TITRE.markdown].

Exemple : 2013-01-07-blog-octopress.markdown

#### Ajouter l'entête

{% gist 4533268 %}

#### Régider votre article

Prenez exemple sur les articles déjà écrits : [ici](https://github.com/JCERTIFLab/jcertiflab.github.com/tree/source/source/_posts).
Profitez pour regarder les sources de cet article pour vous faire une idée.

Pour avoir une preview du blog en local, il faut :

*	Installer Ruby 1.9.3
*	Installer bundler
*	Utiliser la commande : rake preview
*	Lancer le blog via l'url : http://localhost:4000

Plus de détails [ici](http://octopress.org/docs/setup/).

#### Soumettez un article

{% gist 4533333 %}

#### Mise en ligne d'un article

La mise en ligne est effectuée par un build Jenkins. Si vous souhaitez mettre en place ce mécanisme pour votre blog, l'article [Octopress continous integration](http://blog.dlecan.com/octopress-continous-integration/) va vous intéresser.

## Pour une utilisation avancée d'Octopress
Consulter la [documentation en ligne](http://octopress.org/docs/) ou contacter lab@jcertif.org

