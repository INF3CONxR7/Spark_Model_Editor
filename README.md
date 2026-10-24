<p align="center">
  <img src="https://zupimages.net/up/26/43/ei11.png" alt="Logo de Spark Model Editor" width="128">
</p>

<h1 align="center">Spark Model Editor</h1>

<p align="center">
  Ouvrez et modifiez les modèles de <b>Minecraft PlayStation 3 Edition</b> (fichiers <b>models.bin</b>) :<br>arbre des
  modèles, de leurs parties et de leurs boîtes, positions, rotations, décalages de texture, dimensions, UV et échelle.
</p>

<p align="center">
  <a href="https://github.com/INF3CONxR7/Spark_Model_Editor/releases/latest"><img src="https://img.shields.io/github/v/release/INF3CONxR7/Spark_Model_Editor?label=t%C3%A9l%C3%A9charger&color=F6922C" alt="Télécharger"></a>
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?logo=windows&logoColor=white" alt="Windows 10 et 11">
  <a href="https://discord.gg/TbFYvqsh5z"><img src="https://img.shields.io/badge/Discord-rejoindre-5865F2?logo=discord&logoColor=white" alt="Serveur Discord"></a>
</p>

---

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Raccourcis clavier](#raccourcis-clavier)
- [Mises à jour et Discord](#mises-à-jour-et-discord)
- [En cas de problème](#en-cas-de-problème)
- [Désinstaller](#désinstaller)
- [Crédits](#crédits)
- [Support](#support)
- [English](#english)

## Fonctionnalités

- **Ouverture des fichiers models.bin** de Minecraft PS3 par *Fichier > Ouvrir…*, ou par un clic droit sur le fichier,
  *Ouvrir avec Spark Model Editor*. Cette commande n’apparaît que sur les fichiers nommés `models.bin` : les autres
  fichiers `.bin` ne changent pas. Un fichier qui n’est pas un models.bin lisible est refusé avec un message, sans être
  modifié.
- **Arbre des modèles** : le fichier, ses modèles (avec la tête du mob correspondant), leurs parties et leurs boîtes.
  *Outils > Tout développer* et *Tout réduire* ouvrent ou replient tout l’arbre.
- **Inspecteur** de l’élément choisi, à droite :
  - **modèle** : largeur et hauteur de la texture ;
  - **partie** : position (translation X, Y, Z), décalage de texture (X, Y) et rotation (X, Y, Z) ;
  - **boîte** : position, dimensions (longueur, hauteur, largeur), coordonnées de texture (UV) et échelle.
- **Saisie rapide** : tapez une valeur puis `Entrée`, ou faites-la varier avec les petites flèches du champ, les
  touches `Haut` et `Bas` ou la molette (par pas de 1, de 0,1 pour l’échelle).
- **Enregistrement fidèle** : seules les valeurs modifiées changent. Le reste du fichier (noms, ordre des modèles,
  octets réservés) est réécrit à l’identique.
- **Enregistrement sûr** : une copie de l’original (`.bak`) est gardée au premier enregistrement par-dessus, puis le
  fichier écrit est relu pour vérifier qu’il est lisible. Un fichier modifié est signalé dans la ligne d’état
  (« Non enregistré »), et l’application propose de l’enregistrer avant de le fermer.
- **À propos** (`F1`) : version, recherche des mises à jour, notes de chaque version et licences.
- **Mises à jour automatiques** et **présence Discord**.

## Installation

1. Ouvrez la [dernière version](https://github.com/INF3CONxR7/Spark_Model_Editor/releases/latest) et téléchargez
   **`SparkModelEditor-win-x64.zip`** (le fichier `.zip.sig` sert au programme de mise à jour : inutile de le
   télécharger).
2. Extrayez l’archive à l’endroit de votre choix, par exemple dans Documents ou sur le Bureau : vous obtenez le dossier
   **`SparkModelEditor-win-x64`**. Gardez ensemble les deux fichiers qu’il contient.
3. Lancez **`Spark Model Editor.exe`** depuis ce dossier.

Il faut un PC sous **Windows 10 ou 11 (64 bits)**. Rien d’autre à installer : le runtime .NET est inclus dans
l’exécutable.

> **Windows SmartScreen** : l’exécutable n’est pas signé Authenticode, Windows peut donc afficher « Windows a protégé
> votre ordinateur ». Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

## Utilisation

1. **Ouvrir** : *Fichier > Ouvrir…* (`Ctrl+O`), puis choisissez le `models.bin`, ou faites un clic droit sur le
   fichier, *Ouvrir avec Spark Model Editor* (sous Windows 11, dans *Afficher plus d’options*). Travaillez de préférence
   sur une copie tirée de la backup : la copie `.bak` n’est faite qu’une fois.
2. **Choisir un élément** dans l’arbre : un modèle (par exemple `ocelot`), une de ses parties (`head`, `body`…) ou une
   de ses boîtes (`Box 1`…).
3. **Modifier** les valeurs dans l’inspecteur : `Entrée` valide la saisie, les flèches et la molette avancent pas à
   pas.
4. **Enregistrer** : `Ctrl+S`, ou *Enregistrer sous…* (`Ctrl+Maj+S`) pour écrire un autre fichier. Une fois le fichier
   enregistré, la ligne d’état n’affiche plus « Non enregistré ».
5. **Sur la PS3** : remettez le fichier à la place de l’original dans le jeu.

Conseils : notez les valeurs d’origine avant d’expérimenter, changez une valeur à la fois, et gardez à l’esprit que les
rotations sont en degrés (90 = un quart de tour) et que les dimensions des boîtes et de la texture sont des nombres
entiers.

## Raccourcis clavier

| Touche | Action |
|---|---|
| `Ctrl+O` / `Ctrl+S` / `Ctrl+Maj+S` | Ouvrir / Enregistrer / Enregistrer sous |
| `Ctrl+W` | Fermer le fichier |
| `Entrée` | Valider la valeur saisie |
| `Haut` / `Bas` (ou la molette) | Augmenter / diminuer la valeur du champ |
| `F1` / `Échap` | Ouvrir / fermer *À propos* |
| `Alt+F4` | Quitter |

## Mises à jour et Discord

- **Mises à jour** : quelques secondes après le démarrage, l’application vérifie sur GitHub si une nouvelle version est
  publiée. Si c’est le cas, le bouton de la version, en haut à droite, l’annonce en ambre : un clic, et l’application
  propose d’enregistrer le fichier, se ferme, installe la mise à jour, puis se relance. *Infos > Rechercher les mises
  à jour* lance la même vérification. Chaque version est **signée** : une version dont la signature est absente ou
  invalide est refusée.
- **Présence Discord** : si Discord est ouvert, votre profil indique ce que fait l’application (parcourt ou modifie un
  modèle, partie choisie, nombre de modifications, enregistrement), jamais le nom de vos fichiers. Le bouton Discord, à
  gauche de la version, affiche ou masque l’activité.
- Les logos Discord et GitHub de l’en-tête, comme *Infos > Serveur Discord* et *Infos > GitHub*, ouvrent le serveur
  Discord et la page GitHub de l’auteur.

## En cas de problème

| Problème | Solution |
|---|---|
| « Ouverture impossible » | Le fichier n’est pas un models.bin de Minecraft PS3, ou il est tronqué : reprenez-le dans la backup. |
| Un modèle s’affiche mal dans le jeu | Remettez la copie `models.bin.bak` (renommée en `models.bin`), puis refaites les changements un par un. |
| « Le fichier a été écrit mais n’a pas pu être relu » | Ne l’utilisez pas dans le jeu : remettez la copie `.bak` et réessayez. |
| L’enregistrement échoue | Le dossier est peut-être en lecture seule ou le fichier ouvert ailleurs : *Enregistrer sous* dans un autre dossier. |
| Le double-clic sur `models.bin` n’ouvre pas Spark Model Editor | C’est voulu : Windows associe une extension, pas un nom de fichier, et `.bin` sert à beaucoup d’autres fichiers. Faites un clic droit, *Ouvrir avec Spark Model Editor*. |
| La commande *Ouvrir avec Spark Model Editor* n’apparaît pas | Lancez l’application une fois : c’est elle qui ajoute la commande. Le fichier doit s’appeler `models.bin`. Sous Windows 11, ouvrez *Afficher plus d’options*. |

Une question ? Rejoignez le [serveur Discord](https://discord.gg/TbFYvqsh5z).

## Désinstaller

Supprimez le dossier de l’application. Elle garde aussi, pour votre compte Windows :

| Emplacement | Contenu |
|---|---|
| `HKEY_CURRENT_USER\Software\SparkModelEditor` | Réglages (langue, dossier et fichiers récents, activité Discord…). |
| `HKEY_CURRENT_USER\Software\Classes\SystemFileAssociations\.bin\shell\SparkModelEditor` | Commande *Ouvrir avec Spark Model Editor* du clic droit sur `models.bin`. |
| `%LocalAppData%\Spark Model Editor` | Journal des mises à jour. |

Vous pouvez supprimer ces clés et ce dossier.

## Crédits

- **Spark Model Editor** : © 2026 INF3C7ONxR7. Tous droits réservés.
- **Format des modèles (models.bin)** : établi d’après l’étude de Model-Studio (PhoenixARC). La lecture, l’écriture et
  les images (icône, têtes des mobs) sont propres à Spark Model Editor.
- **Logos Discord et GitHub** : tracés de [Simple Icons](https://simpleicons.org/) (CC0) ; ces logos sont des marques
  de leurs propriétaires.

Projet non officiel, sans lien avec Mojang, Microsoft, 4J Studios ni Sony. Minecraft est une marque de Mojang ;
PlayStation et PS3 sont des marques de Sony Interactive Entertainment.

## Support

- Discord : [discord.gg/TbFYvqsh5z](https://discord.gg/TbFYvqsh5z)
- Soutenir le projet : [ko-fi.com/INF3C7ONxR7](https://ko-fi.com/INF3C7ONxR7)

Développé par **INF3C7ONxR7**.

---

## English

**Spark Model Editor** opens and edits the models of **Minecraft PlayStation 3 Edition** (**models.bin** files). The
interface is in French; English texts are included: set the string value `Language` to `en` in
`HKEY_CURRENT_USER\Software\SparkModelEditor` (applied at the next start).

**Requirements**: Windows 10 or 11 (64-bit) PC, nothing else to install (the .NET runtime is included).

**Features**: open a models.bin from *File > Open* (`Ctrl+O`) or by right-clicking it, *Open with Spark Model Editor*
(shown on files named `models.bin` only; other `.bin` files are left alone) ·
tree of the models (with their mob head), parts and boxes, expand or collapse all · inspector for the selected item:
texture width and height (model); translation, texture offset and rotation (part); position, size, UV and scale
(box) · type a value and press `Enter`, or step it with the field arrows, `Up`/`Down` or the mouse wheel · faithful
saving (unchanged data written back byte for byte) · safe saving (original kept as `.bak` the first time, written
file read back) · unsaved changes flagged in the status line, save offered before closing · About window (`F1`) with
release notes · automatic signed updates and Discord presence.

**Install**: download **`SparkModelEditor-win-x64.zip`** from the
[latest release](https://github.com/INF3CONxR7/Spark_Model_Editor/releases/latest) (not the `.sig` file, used by the
updater), extract it to get the **`SparkModelEditor-win-x64`** folder and run **`Spark Model Editor.exe`**. The
executable is not Authenticode-signed, so Windows SmartScreen may show "Windows protected your PC": click **More
info**, then **Run anyway**.

**Uninstall**: delete the app folder. Settings are in `HKEY_CURRENT_USER\Software\SparkModelEditor`, the right-click
command in `HKEY_CURRENT_USER\Software\Classes\SystemFileAssociations\.bin\shell\SparkModelEditor`, the update log in
`%LocalAppData%\Spark Model Editor`.

Unofficial project, not affiliated with Mojang, Microsoft, 4J Studios or Sony.

**Support**: [Discord](https://discord.gg/TbFYvqsh5z) · [Ko-fi](https://ko-fi.com/INF3C7ONxR7) · Developed by
**INF3C7ONxR7**.
