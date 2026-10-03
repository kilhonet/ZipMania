# ZipMania

**Un archiveur gratuit pour Windows, rapide et léger, qui ouvre plus de 50 formats et compresse en 7Z · ZIP · TAR.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · Français

> Ce document est une traduction. En cas de divergence, la [version coréenne](README.ko.md) fait foi.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Source](https://img.shields.io/badge/source-Apache%202.0-lightgrey)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/zipmania?lang=fr)

![Capture d'écran de ZipMania](images/zipmania-en.webp)

## Présentation

ZipMania est un archiveur concentré sur une seule chose : ouvrir et créer des archives. Il lit plus de 50 formats, dont ZIP, RAR, 7Z, EGG, ALZ et ISO, et crée des archives en **7Z · ZIP · TAR**.

Ouvrez une archive : l'arborescence des dossiers s'affiche à gauche et la liste des fichiers à droite. Choisissez uniquement les fichiers dont vous avez besoin et extrayez-les, ou glissez-les directement dans l'Explorateur. Les images sont prévisualisées sans extraction. Un double-clic ouvre un fichier dans le programme associé, et une archive contenue dans une archive s'ouvre dans une nouvelle fenêtre.

Le menu contextuel de l'Explorateur propose des actions en un clic comme « Extraire ici » et « Compresser en *nom*.zip », et un outil en ligne de commande (`zm.exe`) est fourni pour les scripts de sauvegarde et les programmes externes tels que Total Commander. Ni publicité, ni logiciel additionnel.

## Fonctionnalités

- **Ouvre plus de 50 formats** — ZIP, ZIPX, JAR, RAR, 7Z, EGG, ALZ, TAR, GZ, BZ2, XZ, ZST, ISO, IMG, WIM, DMG, MSI, RPM, DEB, CAB, CBZ, CBR et d'autres.
- **Compresse en 7Z · ZIP · TAR** — cinq niveaux de compression, mots de passe, chiffrement des noms de fichiers en 7Z, archives fractionnées.
- **ZIP rapide** — un moteur dédié se charge de la compression et de l'extraction ZIP.
- **Seulement ce qu'il vous faut** — extrayez les fichiers sélectionnés, glissez-les dans l'Explorateur ou ouvrez-les d'un double-clic.
- **Archives dans les archives** — double-clic pour les ouvrir dans une nouvelle fenêtre.
- **Aperçu des images** — JPG, PNG, GIF, WebP, SVG et plus, dans le volet inférieur gauche, sans extraction.
- **Modification d'archives** — ajoutez ou supprimez des fichiers dans les archives 7Z, ZIP et TAR.
- **Vérifier · Analyser** — un tableau CRC indique si l'archive est endommagée, et l'antivirus de Windows (AMSI) peut analyser les fichiers internes.
- **Nettoyage après compression** — vérifie l'archive une fois terminée et ne supprime les originaux que si elle passe le test.
- **Menu contextuel de l'Explorateur** — Extraire ici, Extraire vers *nom*, Compresser en *nom*.zip, Compresser chacun séparément, Extraire chacun dans son dossier.
- **Ligne de commande** — `zm.exe` (console) et `ZipMania.exe` (fenêtre de progression) pour compresser, extraire, lister et tester. Accepte la syntaxe d'options de 7-Zip et de Bandizip.
- **Thème clair/sombre, 9 langues** — suit Windows par défaut, ou choisissez le vôtre.

## Téléchargement / Installation

| Paquet | Lien |
|---|---|
| Installateur | [Télécharger](https://down.kilho.net/zipmania?lang=fr) |
| Portable (ZIP) | [Télécharger](https://down.kilho.net/zipmania?lang=fr&nosetup) |

ZipMania peut être utilisé en version portable : décompressez-le où vous voulez et lancez `ZipMania.exe`. Les réglages sont enregistrés dans `settings.toml` à côté de l'exécutable, ils vous suivent donc sur une clé USB.

## Utilisation

### Premiers pas

**Extraire**

1. Double-cliquez sur une archive, ouvrez-en une avec **[Ouvrir]** dans ZipMania, ou déposez-la sur la fenêtre.
2. Parcourez l'arborescence à gauche et la liste des fichiers à droite. Sélectionnez des fichiers et cliquez sur **[Extraire]**.
3. Dans la fenêtre **Extraire**, choisissez le dossier de destination. Utilisez les raccourcis à gauche (Bureau, Documents, Téléchargements…) ou l'arborescence ; un clic droit sur un espace vide crée un nouveau dossier.
4. Sous **Fichiers à extraire**, choisissez **Tous les fichiers** ou **Fichiers sélectionnés**, puis cliquez sur **[OK]**. La progression, la vitesse et le temps restant s'affichent ; à la fin, **[Ouvrir le dossier]** vous mène au résultat.

**Compresser**

1. Cliquez sur **[Nouvelle archive]** dans la barre d'outils, ou déposez des fichiers et des dossiers sur la fenêtre de ZipMania.
2. La fenêtre **Nouvelle archive** les liste. Ajoutez-en avec **[Ajouter des fichiers]** / **[Ajouter des dossiers]** ou en les déposant.
3. Définissez le **Nom du fichier** (emplacement), le **Format** (7Z · ZIP · TAR) et, si besoin, **Définir un mot de passe**, **Fractionner**, les actions **Après** et la **Méthode**.
4. Cliquez sur **[Démarrer]**. À la fin, **[Ouvrir le dossier]** ou **[Fermer]**.

Pour le faire directement depuis l'Explorateur, utilisez le menu contextuel — voir « Comment… » ci-dessous.

### La fenêtre

| Bouton de la barre | Rôle |
|---|---|
| **Ouvrir** | Ouvrir une archive |
| **Extraire** | Extraire l'archive ouverte (ou seulement les fichiers sélectionnés) |
| **Nouvelle archive** | Choisir des fichiers et dossiers et créer une nouvelle archive |
| **Ajouter des fichiers** / **Supprimer des fichiers** | Ajouter ou retirer des fichiers de l'archive ouverte (7Z · ZIP · TAR uniquement) |
| **Vérifier** | Contrôler si l'archive est endommagée (CRC) |
| **Analyser** | Analyser les fichiers internes avec l'antivirus de Windows (fichiers de moins de 10 Mo) |
| **Vue à plat** | Afficher tous les fichiers dans une seule liste avec leur chemin complet, sans dossiers |
| **Paramètres** | Thème, langue, réglages d'extraction, associations de fichiers, menu de l'Explorateur |

- **Arborescence (en haut à gauche)** — cliquez sur un dossier pour afficher ses fichiers à droite.
- **Aperçu (en bas à gauche)** — apparaît lorsqu'un seul fichier image est sélectionné.
- **Liste des fichiers** — Nom · Taille · Taille compressée · Type · Modifié. Cliquez sur l'en-tête Nom, Taille ou Modifié pour trier ; faites glisser les bordures pour redimensionner les colonnes.
- **Barre d'état** — nombre d'éléments, nombre et taille des fichiers sélectionnés, taille compressée et taux.
- Faites glisser le séparateur pour redimensionner l'arborescence et la liste. La taille de la fenêtre et l'état agrandi sont restaurés à la prochaine ouverture.

### Comment…

**Extraire directement depuis l'Explorateur**
Faites un clic droit sur une archive pour voir les entrées ZipMania.
- **Extraire ici** — extrait dans le dossier de l'archive sans rien demander. Activez **Fermer la fenêtre** dans la fenêtre de progression pour qu'elle se ferme dès la fin.
- **Extraire vers « nom »** — crée un nouveau dossier au nom de l'archive et y extrait le contenu. Idéal pour les archives contenant beaucoup de fichiers.
- **Extraire avec ZipMania…** — ouvre la fenêtre où vous choisissez la destination et les options.
- **Ouvrir avec ZipMania** — pour regarder le contenu d'abord.

Avec **plusieurs archives sélectionnées**, **Extraire ici** les extrait l'une après l'autre, et **Extraire chacun dans son dossier** place chaque archive dans un dossier portant son nom.

**Compresser directement depuis l'Explorateur**
Faites un clic droit sur des fichiers ou des dossiers.
- **Compresser en « nom.zip »** — crée un ZIP sur place sans rien demander. Un seul dossier prend le nom du dossier ; plusieurs éléments prennent le nom du dossier courant. Si le nom existe déjà, un numéro est ajouté : `nom (2).zip`.
- **Compresser avec ZipMania** — ouvre la fenêtre pour choisir le format, le mot de passe, le fractionnement, etc.
- **Compresser chacun séparément** — crée un ZIP par élément sélectionné, à son nom. Pratique pour archiver plusieurs dossiers individuellement.

**Ne sortir que quelques fichiers d'une archive**
Trois façons :
- Sélectionnez les fichiers (Ctrl/Maj pour plusieurs) et cliquez sur **[Extraire]** → **Fichiers à extraire : Fichiers sélectionnés**.
- Clic droit sur la sélection → **Extraire les fichiers sélectionnés**.
- **Glissez la sélection dans l'Explorateur ou sur le Bureau** — elle est extraite sur place.

**Ouvrir un fichier interne sans extraire**
Double-cliquez ou appuyez sur Entrée ; il s'ouvre dans le programme associé (les documents dans votre éditeur, les vidéos dans votre lecteur). Clic droit → **Exécuter le fichier** fait la même chose. Les copies temporaires sont nettoyées à la fermeture de ZipMania.

**Une archive dans une archive**
Double-cliquez dessus : elle s'ouvre dans une **nouvelle fenêtre**. Vous pouvez garder plusieurs fenêtres ouvertes et passer de l'une à l'autre.

**Feuilleter des photos dans une archive**
Sélectionnez un fichier image (JPG · PNG · GIF · BMP · WebP · ICO · SVG · TIFF · AVIF) et un aperçu apparaît en bas à gauche. Utilisez les flèches pour les faire défiler. Les images de plus de 32 Mo affichent un message au lieu de l'aperçu.

**Les dossiers profonds compliquent la recherche**
Activez **[Vue à plat]** dans la barre : les dossiers disparaissent et chaque fichier est listé avec son chemin. Triez par nom, taille ou date pour trouver aussitôt les fichiers les plus gros ou les plus récents. Cliquez à nouveau pour revenir à la vue par dossiers.

**Archives protégées par mot de passe**
Une demande de mot de passe apparaît à l'ouverture. Un mot de passe erroné est redemandé ; un mot de passe correct est mémorisé pour cette archive, si bien que l'aperçu, l'ouverture et l'extraction ne le redemandent pas. Si un fichier protégé se présente pendant l'extraction, il est demandé à ce moment-là ; laissez vide et seul ce fichier est ignoré, le reste continue.

**Compresser avec un mot de passe**
Dans la fenêtre **Nouvelle archive**, cliquez sur **[Définir un mot de passe]** et saisissez-le.
- Avec **7Z**, vous pouvez aussi activer **Chiffrer les noms de fichiers** — sans le mot de passe, personne ne peut même voir ce qu'il y a dedans.
- **ZIP** n'accepte que des lettres et des chiffres. Un mot de passe non ASCII affiche un avertissement et ne démarre pas — passez en 7Z ou utilisez un mot de passe ASCII.
- **TAR** ne prend pas en charge les mots de passe.

**Envoyer un gros fichier par e-mail ou messagerie**
Sous **Fractionner**, choisissez 10 Mo · 25 Mo · 100 Mo · 700 Mo · 1 Go · 4 Go, ou choisissez **Personnalisé…** et tapez par exemple `700M` ou `4GB`. L'archive est enregistrée en `nom.7z.001`, `.002`, … (7Z · ZIP). Le destinataire place les parties dans un même dossier et ouvre ou extrait **uniquement le fichier `.001`**.

**Supprimer les originaux après compression pour libérer de l'espace**
Sous **Après**, activez **Vérifier l'archive** et **Supprimer les sources**. Les sources ne sont supprimées que lorsque chaque fichier a été stocké et que la vérification a réussi : une archive défectueuse ne vous coûtera jamais les originaux.

**Compresser plusieurs dossiers séparément**
Placez les dossiers dans la fenêtre **Nouvelle archive** et activez **Compresser chaque élément dans sa propre archive**. Chaque dossier obtient une archive à son nom, à côté de lui. C'est la même chose que **Compresser chacun séparément** de l'Explorateur, mais ici vous pouvez aussi choisir le format et un mot de passe.

**Plus vite ou plus petit**
La **Méthode** a cinq niveaux : **Stocker (sans compression)** · **Rapide** · **Normal** · **Élevé** · **Maximum**. Pour simplement regrouper des photos ou des vidéos déjà compressées, **Stocker** est le plus rapide ; pour des documents et du code source, qui se compressent bien, **Élevé** ou **Maximum** est payant. Pour le résultat le plus petit, utilisez le format **7Z** (par défaut).

**Ajouter ou retirer des fichiers d'une archive existante**
Avec une archive 7Z · ZIP · TAR ouverte :
- Cliquez sur **[Ajouter des fichiers]** ou déposez des fichiers sur la fenêtre — répondez Oui à « Ajouter N fichier(s) à … ? ».
- Sélectionnez des fichiers et cliquez sur **[Supprimer des fichiers]** ou clic droit → **Supprimer des fichiers**.
Les autres formats (RAR, EGG, …) ne sont pas modifiables : les boutons sont désactivés.

**Vérifier qu'une archive téléchargée est intacte**
Cliquez sur **[Vérifier]** : le CRC attendu et le CRC réel de chaque fichier sont comparés et présentés dans un tableau. Les archives endommagées ou partiellement téléchargées sont repérées avant l'extraction.

**Vérifier qu'une archive téléchargée est sûre**
**[Analyser]** confie les fichiers internes à l'antivirus de Windows (AMSI) sans les extraire. Les fichiers de 10 Mo ou plus sont ignorés, et un antivirus avec protection en temps réel doit être actif. Le résultat indique pour chaque fichier Sain · Menace · Ignoré.

**Un fichier du même nom existe déjà lors de l'extraction**
La question est posée pour chaque fichier : **Écraser** · **Ignorer** · **Renommer**. Activez **Appliquer à tous les fichiers restants** pour réutiliser la même réponse.

**L'extraction a éparpillé des fichiers dans le dossier**
**Créer un sous-dossier au nom de l'archive** est activé par défaut, les fichiers vont donc dans un dossier portant le nom de l'archive. Pour extraire directement, désactivez-le dans la fenêtre **Extraire** ou dans **Paramètres → Extraction**, ou utilisez **Extraire ici** de l'Explorateur.

**Supprimer l'archive et ouvrir le dossier une fois terminé**
Dans **Paramètres → Extraction**, activez **Supprimer l'archive après une extraction réussie**, **Ouvrir le dossier de destination après l'extraction** et **Fermer la fenêtre d'extraction après l'extraction**. Ces options se changent aussi à chaque fois dans la fenêtre Extraire. L'archive n'est supprimée que si l'extraction a réussi.

**Ouvrir les archives dans ZipMania par double-clic**
Cochez les extensions dans **Paramètres → Association de fichiers**. Si un autre programme possède déjà une extension, **[Non appliqué]** s'affiche ; cliquez dessus pour ouvrir le sélecteur d'applications par défaut de Windows et choisir ZipMania. Lorsque ZipMania ouvre une archive et affiche en haut « Faire de ZipMania l'application par défaut pour les fichiers … ? », vous pouvez changer directement là.

**ZipMania n'apparaît pas dans le menu contextuel**
Dans **Paramètres → Menu de l'Explorateur**, activez **Ajouter compresser/extraire de ZipMania au menu contextuel de l'Explorateur**. Sous Windows 11, il apparaît dans le menu principal ; si vous ne le voyez pas, regardez sous **Afficher plus d'options** (Maj+F10).

**Ouvrir le dossier de l'archive / supprimer l'archive**
Faites un clic droit sur un espace vide de la liste pour **Ouvrir le dossier contenant** et **Supprimer l'archive**. Après avoir vérifié le contenu, vous pouvez supprimer une archive devenue inutile sans quitter ZipMania.

**Piloter la liste au clavier**
Flèches · Page Haut/Bas · Début/Fin pour se déplacer, Maj pour une plage, Ctrl+clic pour ajouter des éléments un à un, **Ctrl+A** pour tout sélectionner, Entrée pour entrer dans un dossier ou ouvrir un fichier, Échap pour fermer la boîte de mot de passe ou de rapport.

**Mode sombre et langue**
Les deux suivent Windows par défaut. Dans **Paramètres → Général**, choisissez le thème (Système · Clair · Sombre) et la langue (한국어 · English · 日本語 · 中文 · Русский · Italiano · Français · Español · العربية) ; les changements s'appliquent immédiatement. Le menu de l'Explorateur utilise la même langue.

**Scripts de sauvegarde et Total Commander**
Deux exécutables sont fournis.
- **`zm.exe`** — écrit dans la console. cmd, PowerShell et les fichiers batch attendent la fin et reçoivent un code de sortie (0 succès / 1 avertissement / 2 erreur).
- **`ZipMania.exe`** — exécute les mêmes commandes avec une **fenêtre de progression**. Adapté aux contextes sans console, comme Total Commander.

```
<exe> a|c [options] <archive> <entrées...>   compresser (a ajoute à une archive existante)
<exe> x|e [options] <archive> [éléments...]  extraire (x conserve les dossiers, e fichiers seuls)
<exe> bx  [options] <archives...>            extraire chaque archive dans un dossier à son nom
<exe> l   [options] <archive>                lister
<exe> t   [options] <archive>                test d'intégrité
```

| Option | Signification |
|---|---|
| `-l:0..9` / `-mx9` | Niveau de compression |
| `-fmt:zip\|7z\|tar` / `-t7z` | Format (par défaut selon l'extension) |
| `-v:700M` / `-v700m` | Taille des volumes |
| `-p:motdepasse` / `-pmotdepasse` | Mot de passe |
| `-o:dossier` / `-odossier` | Dossier de destination |
| `-target:auto\|name\|none` | Extraire dans un sous-dossier au nom de l'archive (`auto` = seulement s'il y a plus d'un élément de premier niveau) |
| `-aoa` `-y` / `-aos` / `-aou` | En cas de nom identique : écraser / ignorer / enregistrer en `nom (2)` |
| `-testdst` | Vérifier l'archive après compression |
| `-delsrc` / `-sdel` | Supprimer les sources si la vérification réussit |
| `-date` | Remplacer `%Y %y %m %d %H %M %S` dans le nom par l'heure actuelle |

Exemples :

```
zm c -l:9 -fmt:7z -testdst -delsrc -date "backup_%y%m%d_%H%M.7z" "D:\Work"   sauvegarde 7Z datée, vérifier puis supprimer les sources
zm a -mx9 -psecret backup.7z D:\Work                                       syntaxe 7-Zip, ajouter à une archive existante
zm x -o:D:\Out -target:auto backup.7z                                      extraire dans un dossier au nom de l'archive
zm bx a.zip b.7z                                                            extraire dans a\ et b\ respectivement
zm l backup.7z.001                                                          lister la première partie d'une archive fractionnée
```

Lancez `zm` sans argument pour l'aide. Dans un fichier batch, écrivez `%` sous la forme `%%`. Pour une commande utilisateur Total Commander, mettez `zm.exe` en commande et `c -l:9 -fmt:7z -aou -testdst -delsrc -date "%T%S %y%m%d_%H%M".7z "%P%S"` en paramètres pour compresser les éléments sélectionnés dans un 7Z daté placé dans le dossier du panneau opposé.

## Configuration

Tout se règle dans **Paramètres** (bouton le plus à droite de la barre) et s'enregistre immédiatement. **[Réinitialiser]** rétablit toutes les valeurs par défaut.

| Catégorie | Élément | Par défaut |
|---|---|---|
| Général | Thème (Système · Clair · Sombre) | Système |
| Général | Langue (Système + 9 langues) | Système |
| Extraction | Créer un sous-dossier au nom de l'archive | Activé |
| Extraction | Supprimer l'archive après une extraction réussie | Désactivé |
| Extraction | Ouvrir le dossier de destination après l'extraction | Désactivé |
| Extraction | Fermer la fenêtre d'extraction après l'extraction | Désactivé |
| Association de fichiers | Extensions ouvertes dans ZipMania par double-clic (zip · 7z · rar · tar · gz · tgz · bz2 · xz · egg · alz · cbz) | Associées par l'installateur |
| Menu de l'Explorateur | Ajouter compresser/extraire de ZipMania au menu contextuel de l'Explorateur | Activé par l'installateur |

Les cases **Fermer la fenêtre** et **Ouvrir le dossier** des fenêtres Nouvelle archive et Extraire mémorisent votre dernier choix.

## Configuration requise

- Windows 10 ou Windows 11, **64 bits**
- Aucun runtime ni composant supplémentaire n'est nécessaire.
- Internet n'est utilisé que pour vérifier l'existence d'une nouvelle version. La compression et l'extraction fonctionnent hors ligne.

## Mises à jour

ZipMania **ne** se met **pas** à jour tout seul. Au démarrage, il vérifie s'il existe une nouvelle version et se contente de vous prévenir ; les nouvelles versions sont publiées manuellement après vérification interne et annoncées sur la [page ZipMania](https://kilho.net/zipmania). Consultez l'[avis sur la politique de mise à jour](https://en.kilho.net/archives/notice/2940).

## Compiler depuis les sources

Le code source est public sur [github.com/newkilho/ZipMania](https://github.com/newkilho/ZipMania) (Rust 1.88 ou plus récent). Le moteur d'archives, `crates/zipmania-archive`, se compile et se teste avec le seul dépôt :

```
cargo test -p zipmania-archive
```

L'application (`app/`) dépend d'un moteur graphique maison et de bibliothèques partagées situés hors du dépôt : l'exécutable ne peut donc pas être compilé à partir du seul dépôt.

## Contribuer

Les rapports de bugs et les suggestions sont les bienvenus via les issues GitHub ou le [forum](https://kilho.top/forum/qna).

## Licence

Le programme ZipMania est un **freeware**. Utilisez-le où vous voulez — à la maison, au travail, à l'école et dans les administrations — et redistribuez-le librement sous sa forme non modifiée.

Le code source est publié sous **Apache License 2.0** ; les crates réutilisables de `crates/` sont disponibles sous MIT ou Apache-2.0, au choix. Les noms « ZipMania » et « 집매니아 » ainsi que les logos et icônes sont des marques de Kilho.net et ne sont pas couverts par la licence — distribuez les versions modifiées sous un autre nom et une autre icône. Les composants open source, dont `7z.dll` de 7-Zip (LGPL), sont listés dans `THIRD-PARTY-NOTICES.txt` dans le dépôt.

## Liens

- Site web : <https://kilho.net/zipmania>
- Code source : <https://github.com/newkilho/ZipMania>
- Forum : <https://kilho.top/forum/qna>
- X (Twitter) : <https://www.twitter.com/kilhonet>

© KILHO.NET
