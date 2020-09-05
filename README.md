# ianRip

Ce script permet de **dématérialiser un DVD (non-protégé)**, c'est-à-dire convertir le film qu'il contient en fichier vidéo, dans l'objectif d'avoir des **copies numériques personnelles de films** pour le cas où on perd le DVD (rayures, casses, vols, etc.).

Ce script a été conçu uniquement pour les distributions _Linux_. Votre machine doit évidemment **posséder un lecteur DVD** interne ou externe pour que le script fonctionne correctement.

## Auteur

**Yann LE COZ** - Bordeaux Ynov Campus Informatique - [ianlcz](https://github.com/ianlcz)

## Sommaire

- [Installation](#installation)
  - [Prérequis](#prérequis)
- [Utilisation](#utilisation)
- [**Licence GNU**](#licence)

## Installation

- ### Prérequis

  Pour pouvoir utiliser ce script, vous devez tout d'abord installer sur votre machine les paquets suivants:

  - **libdvd-pkg** afin d'utiliser le lecteur DVD de votre machine
  - **lsdvd** pour récupérer les informations du DVD
  - **handbrake-cli** pour ripper des DVD en ligne de commande

**1. Clonez le dépôt dans le répertoire de votre choix**

```sh
$ cd <LE_RÉPERTOIRE_DE_VOTRE_CHOIX>
$ git clone https://github.com/ianlcz/ianRip.git
```

**2. Dirigez-vous ensuite dans ce dépôt et donnez l'autorisation d'exécution du script `./ianRip`**

```sh
$ cd ianRip/
$ chmod +x
```

> 🧑‍💻Vous venez de correctement installer le script.

## Utilisation

**1. Pour utiliser le script, dirigez-vous dans le dépôt et exécutez le script**

```sh
$ cd ianRip/
$ ./ianRip
```

Il devra alors s'afficher les informations suivantes en fonction de votre DVD :

```sh
Titre du film :   Interstellar
Qualité :         Super HQ 1080p30 Surround
Format :          mp4
Piste audio :     Français
                  Anglais
                  Espagnol
Son :             dtshd
Mixage audio :    5.1

Voulez-vous changer des paramètres ? [O/N]
>
```

**2. Suivez les instructions qui s'affichent sur votre Terminal et à attendre quand s'affiche le message suivant :**

```sh
Encodage en cours, cela peut prendre quelques heures...
Encoding: task 2 of 2, 22.86 % (15.54 fps, avg 17.40 fps, ETA 02h54m08s)
```

Une fois la dématérialisation effectuée, vous devriez obtenir un message qui vous indique où se trouve votre film en `.mp4` :

```sh
Encodage terminé !
Interstellar.mp4 est dans ~/Vidéos/movies_storage
```

## Licence

Ce programme est sous licence [GNU](./LICENSE)
