# French Macbook Keyboard Layout For Windows (fmbkl4w) 1.1.0
par Nicolas Leclerc <nl@spirotron.fr>

## I. Objectif

Ce projet vise à remédier à l’absence de fichier de définition windows pour les claviers
de Macbook français et par extension les petits clavier alu d'Apple (avec ou sans fil).
Il est important de noter que le grand clavier alu (avec pavé numérique) n’est pas supporté.

## II. License

Le fmbkl4w est sous license GPL v3.0.
Vous trouverez sa description complète dans le fichier gpl-3.0.txt ou bien à l'adresse :
http://www.gnu.org/licenses/gpl.html

## III. Installation

Pour commencer vous devez vous procurer le package d’installation

- soit en le téléchargeant à l’adresse : https://github.com/nleclerc/fmbkl4w/releases
- soit en le compilant à partir des sources (voir plus bas).

Une fois ce package décompressé ou compilé, il vous suffit d’exécuter le fichier setup.exe
et de suivre les instructions.

Il est possible qu'il soit nécessaire de redémarrer windows après l'installation.

## IV. Compilation

Pour compiler le fichier klc vous aurez besoin du Microsoft Keyboard Layout Creator (mklc).
Celui-ci est disponible à l'adresse:
https://www.microsoft.com/en-us/download/details.aspx?id=102134

Une fois installé, vous n’aurez qu’à l’exécuter et ouvrir le fichier fmbkl4w.klc.
Une fois chargé il vous suffit d’aller de faire project/Build DLL and Setup Package
pour que l’installeur soit généré dans votre dossier Mes Documents.

## V. Problèmes Connus

- La rangée de touches numériques ne fonctionne pas comme sur mac quand capslock est activé. Capslock est l'équivalent de shift sous windows malheureusement.

- Les combinaisons de alt+shift avec capslock activé ne sont pas nécessairement correctes.

- Sur certains claviers, il faut utiliser la touche alt de droite pour pouvoir faire des combinaisons (par exemple pour les caracètres `\`, `|`, `~`…)

- A noter que si vous utilisez un PC lambda (et non un mac sous bootcamp), il est quasi indispensable
  d’installer malgré tout les drivers de clavier bootcamp afin que certaines combinaisons fonctionnent
  (comme fct+backspace). Vous devrez extraire le driver seul du package bootcamp général en décompressant
  l’ensemble avec par exemple 7-zip.

  Les drivers bootcamp sont disponibles à l’adresse : http://support.apple.com/fr_FR/downloads/#macoscomponents

  Vous pouvez aussi utiliser Brigadier : https://github.com/timsutton/brigadier
