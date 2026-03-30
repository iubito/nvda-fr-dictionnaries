# nvda-fr-dictionnaries
NVDA speech and symbols dictionnaries, focused on French language, using IBMTTS.

## Short introduction for non-francophone users
* symbols-en.dic: with the huge help of Brian Vogel, you'll find here japanese, cyrillic and greek characters,  programming and maths symbols (`==`, `!=`, `>=`, `&&`, `||`, `⩽`, `∈`...)
* speechdicts: you may find interesting regexp in numeric files, `!` and `_`, spreadsheet cells, CamelBumps and diacritics).

# Dictionnaire de prononciation des mots et symboles pour NVDA

## Thématiques du dictionnaire
* Programmation :
  * Je suis développeur de scripts et applications, dans différents langages de programmation. La programmation utilise en grande majorité des termes anglais. J'ai donc ajouté ces termes dans le dictionnaire. Par exemple : open, select, update, enable, delete.
  * Les mots séparés par des soulignés (underscore) ou collés avec des majuscules (enDosDeChameau, CamelBumps) sont "découpés" afin d'être prononcés convenablement. Exemple : `myObject.getProperty()`, `my_object.get_name()`.
  * Le point d'exclamation est utilisé pour la négation, le double esperluette pour le "et" logique (and), le double barre verticale pour le "ou" logique (or), le double égal pour le teste d'égalité entre 2 valeurs, le triple égal pour l'égalité stricte en PHP... la prononciation de symboles et une regexp bien placée permettent d'entendre convenablement : `if (!expression)`, `if (!(a && b))`, `if (!a || !b)`, `if (a >= b)`...
  * J'ai mis aussi les noms de fonctions et constantes en langages dérivés du C, les noms de balises HTML, de propriétés CSS. Exemple : `sprintf()`, `ksort()`, `memcpy()`, `<title>`, `<textarea>`, `background`, `1.5em`...
  * Liste des langages pleinement supportés : Batch, C, HTML, Java, LaTeX, LibreOffice Math, Lua 4.0, [Harmony Assistant](https://www.myriad-online.com/en/products/harmony.htm) MyrScript, SQL ;
  * Langages partiellement supportés / non vérifiés en intégralité : PHP et dérivés du C, [Reaper](https://www.reaper.fm/download.php) API ;
  * Tableur, fonctions en français et anglais : Excel 2024, Google Sheets, Libre Office Calc ;
* Musique :
  * Je suis musicien, j'utilise des logiciels en anglais et en français, sur des partitions je peux avoir des noms d'instruments dans les 2 langues. J'ai donc ajouté des termes techniques et des noms d'instruments dans le dictionnaire : quarter (une noire), take (une prise), violin (violon), snare (caisse claire), hi-hats (cymbales Charleston), Hohner (une marque d'accordéon), Xfer (nom d'un VST)... ainsi que la prononciation d'instruments du monde : bağlama, banjo, cavaquinho, cheng, çura, marimba...
  * Noms de compositeurs : Wolfgang Amadeus, Beethoven, Schubert, Ligeti, Brassens...
* Cellules de tableur jusqu'à la colonne ZZ ;
* Symboles mathématiques, et un traitement spécial pour le point d'exclamation après un chiffre qui est la factorielle.
* Français :
  * Les adverbes pouvaient être mal prononcer après certains mots. Exemple : Je pense à toi tendrement.
  * Mots d'origine étrangère : bulldozer, bug, crumble, djembé, jazz, popup, scanner...
  * Le e mangé au milieu du verbe épeler
  * ... et quelques corrections sur des mots trouvés par hasard.
* Langues étrangères :
  * Anglais : verbes et mots  fréquents ou techniques, verbes irréguliers ;
  * Caractères diacrités et spéciaux de l'alphabet latin: prononciation lorsque isolé, et quelques caractères transformés dans un mots pour langues ibériques, slaves, roumain et nordiques, exemple : España [Espagna], João [Jo-an-o], Dvořák	[Dvorjak], Bregović (Brégovitsh], Kruševo [Krouchévo], Čoček (Tchotchek], Bokmål...
  * Caractères mathématiques servant au formatage de texte (gras, italique, script), abusément utilisés sur les réseaux sociaux.
  * Caractères japonais : je ne connais pas la langue, mais d'après Wikipédia, j'ai fait une approximation de la prononciation dans le fichier des symboles ;
  * Alphabets grec et cyrillique : ici, aucune tentative de prononciation, mais j'ai tenu à mettre ces caractères pour épeler un mot en se déplaçant caractère par caractère, ou pour entendre une anomalie si un pirate remplace un caractère latin par un caractère cyrillique ressemblant. Cela permet de détecter un spam lorsque cette technique est utilisée. NVDA dira "a cyrillique", "d cyrilliquemajuscule ", etc.
* Noms propres :
  * pays et capitales : Bahrein, London ;
  * états américains : Iowa, Maryland, Ohio ;
  * régions et villes de France, Allemagne, Grande-Bretagne, USA ;
  * quelques villages imprononçables d'Auvergne ! Arlempdes, Cunlhat, Mézenc ;
  * Prénoms : Aya, Kylian, Owen...
  * physiciens, chimistes qui ont donné leur nom à des unités de mesure : Newton, Fahrenheit, Kelvin, Siemens...
* Termes en rapport avec la finance (types de comptes bancaires, brokers, paires Forex, crypto-monnais) ;
* Quelques acronymes administratifs français.
* Noms de fabricants, de logiciels, de réseaux sociaux, applications en ligne : BitDefender, Facebook, Samsung...

Avant tout, j'ai tenu à ce qu'un texte français soit correctement prononcé. Il y a donc des termes anglais ou techniques qui ne sont pas traités. Par exemple :
* `file` = fichier en anglais, mais aussi une file d'attente, ou « il file à l'anglaise » ;
* `border` = bordure en CSS, frontière en anglais, et le verbe border en français ;
* le verbe `try` (essayer en anglais) est traité, ainsi que sa forme passée `tried`, mais pas le nom au pluriel `tries` (des essais), car c'est le verbe trier à la deuxième personne du singulier en français.

Ce dictionnaire m'est utile au quotidien, et le sera pour mon fils qui va être équipé d'un ordinateur au collège, qui va donc apprendre du français, des mathématiques, de la chimie, de la musique... et utiliser Libre Office pour écrire des formules.


## Optimisé pour le synthétiseur IBMTTS
Le synthétiseur IBMTTS, qui n'est pas tout à fait un addon officiel, est selon moi le plus efficace en terme de temps de réponse, et qui n'apporte pas de reconstitution des acronymes en noms à rallonge comme le font les voix de synthèse de Microsoft.

Instructions pour télécharger, installer et utiliser IBMTTS :
1. Allez sur [BlindHelp](https://blindhelp.net/software/ibmtts)
2. Recherchez le titre niveau 2 "Downloads" ou scrollez jusqu'à la fin de la page.
3. Téléchargez le deuxième lien qui ressemble à quelque chose comme "Download IBMTTS-V25.1.1 Packaged with Libraries (8.79 MB)"
4. C'est un fichier ZIP qui contient un répertoire.
5. Double cliquez ou Entrée sur le fichier dont le nom ressemble à "IBMTTS-25.1.1-by-BHP.nvda-addon"
6. C'est l'installation classique d'un add-on de NVDA.
7. Dans les paramètres de NVDA, catégorie Parole, choisissez le synthétiseur IBMTTS
8. Paramétrez à votre guise la voix, le débbit. La voix Glen est la plus couramment utilisée.
9. Décochez "Activer l'extension des abbréviations"
10. Décochez "Changement automatique de langue". En effet, si cela s'avère intéressant sur le papier, il faut savoir que beaucoup de sites sont mal codés et indiquent langue anglaise alors que le contenu est en français, et à l'opposé, des logiciels en anglais n'indiqueront jamais qu'ils sont en anglais. On va donc rester en français, des raccourcis permettent de changer de langue, et on va alimenter le dictionnaire pour que les mots les plus fréquents en anglais soient à peu près prononcés correctement, "with a French accent, oeuf corse!"
11. Niveau de ponctuations et symboles : "quelques uns".


## Comment utiliser mes fichiers ?

1. Dans la barre d'adresse de l'explorateur de fichier, ou par menu Démarrer > Exécuter, aller dans le répertoire `%APPDATA%\NVDA`.

### Prononciation des symboles

2. Si le fichier `symbols-fr.dic` existe, renommez-le.
3. Téléchargez [symbols-fr.dic](https://github.com/iubito/nvda-fr-dictionnaries/raw/refs/heads/main/symbols-fr.dic) dans ce répertoire.
4. Si vous aviez personnalisé ou ajouté la prononciation de symboles, éditez le fichier `symbols-fr.dic` avec un éditeur de texte (Notepad++ recommandé), remplacez ou ajoutez vos lignes personnalisées.

### Dictionnaire

5. Allez dans le répertoire `speechdicts` (donc `%APPDATA%\NVDA\speechdicts`).
6. Si vous avez déjà ajouté des prononciations, repérez le fichier `.dic` récemment modifié  Sinon, créez un fichier `default.dic`.
7. Éditez-le, idéalement avec Notepad++.
8. Téléchargez ou copiez-collez le contenu mes fichiers présents dans [speechdicts](https://github.com/iubito/nvda-fr-dictionnaries/tree/main/speechdicts), en les prenant dans l'ordre numérique puis alphabétique : 01, 02... et terminez par fr

## Liste des fichiers speechdicts

J'ai découpé mon fichier `default.dic` en plusieurs sections, ainsi vous pouvez ne prendre que celle qui vous intéressent. Au final, toutes doivent être copiées dans un même fichier.

|Fichier|Contenu|
|-|-|
|[01 !_dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/01%20!_.dic)|<ul><li>Le point d'exclamation peut se prononcer "not" devant une variable ou une fonction en programmation.</li><li>Le point d'exclamation après un chiffre se prononce "factorielle". ` 4! = 4×3×2×1`.</li><li>Le _ (souligné) seul est prononcé, au milieu d'un mot il le découpe. Ainsi, chaque mot est traité par la suite du dictionnaire.</li></ul>|
|[02 Cellules de tableur.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/02%20cellules%20de%20tableur.dic)|1 ou 2 caractères alpha majuscule, suivi d'un nombre, c'est le nom d'une cellule dans Excel / LibreOffice Calc / Google Sheets.<br>Les caractères alpha sont décomposés.<br>Exemple : `AU1` prononcé "= a u 1" et non "au 1".|
|[03 CamelBumps.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/03%20CamelBumps.dic)|Des expressions régulières pour séparés les mots collés commençant par une majuscule. Usage principal en programmation, mais aussi des noms de logiciels ou d'entreprises.<br>Les mots ainsi séparés sont traités par la suite du dictionnaire.<br>Exemple : MakeMusic, iPhone, `theTextarea.selectAll()`, `GUIAddButton`.|
|[04 extensions.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/04%20extensions.dic)|Brève liste d'extensions de fichiers.|
|[05 mots composés.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/05%20mots%20compos%C3%A9s.dic)|Quelques mots composés qui pourraient être mal prononcés si mis dans la liste principale. Par exemple<ul><li>add-on, le mot "on" n'est pas traité tout seul,</li><li>can't doit être traité incluant l'apostrophe et le t pour ne pas être traité comme can puis t.</li></ul>|
|[06 AA-ZZ.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/06%20AA-ZZ.dic)|Tous les mots de 2 lettres sont traités ici. Si ce ne sont pas des mots français/anglais, alors les 2 lettres sont prononcées séparément (épellation) comme un sigle ou le nom d'une droite ou d'un vecteur en géométrie.<br>Les majuscules et minuscules sont traitées. Exemple, AD peuten majuscule  être une droite passant par les points A et D, mais aussi l'acronyme de Active Directory. Avec une miniscule ou tout en minuscule, cela peut être dans une expression latine "Ad libitum", "Ad vitam aeternam".|
|[07 dates.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/07%20dates.dic)|Lorsqu'une date est au format ISO, c'est-à-dire année-mois-jour, ce traitement raccourcis les silences entre chaque élément. J'utilise beaucoup ce format de date pour trier des fichiers par ordre alpha et chronologique en commençant leur nom par la date dans ce format.|
|[08 diacritics.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/08%20diacritics.dic)|Des caractères Latin-1 et -Latin-2 étendus, avec des accents, caron, hatchek, cédille... Lorsqu'ils sont isolés, ils sont prononcés (par exemple S cédille), lorsqu'on se déplace par caractère, il est possible que le mot cédille soit épelé.<br>Lorsqu'ils sont dans un mot, certains caractères sont transformés lorsque leur prononciation est constante. Le ñ (n tilde) espagnol (au détriment du breton), le ã (a tilde) portugais, le č (c hatchek) des langues slaves transformé en tch.|
|[09 A-Z variantes.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/09%20A-Z%20variantes.dic)|Des outils permettent de formatter du texte en gras, italique, script, en utilisant des caractères mathématiques, pour poster sur les réseaux sociaux.<br />Ces règles les transforment en caractères latins pour être prononcés correctement.|
|[fr.dic](https://github.com/iubito/nvda-fr-dictionnaries/blob/main/speechdicts/fr.dic)|La liste principale du dictionnaire, trié par ordre alphabétique.|

Faites-en bon usage ! ☺
