# nvda-fr-dictionnaries
NVDA speech and symbols dictionnaries, focused on French language, using IBMTTS.

## Short introduction for non-francophone users
* symbols-fr.dic: you'll find here japanese, cyrillic and greek characters, and programming-specific symbols (==, !=, >=...)
* speechdicts: you may find interesting regexp in numeric files, ! and _, spreadsheet cells, CamelBumps and diacritics).

# Dictionnaire de prononciation des mots et symboles pour NVDA

## Thématiques du dictionnaire
* Programmation :
  * Je suis développeur de scripts et applications, dans différents langages de programmation. La programmation utilise en grande majorité des termes anglais. J'ai donc ajouté ces termes dans le dictionnaire. Par exemple : open, select, update, enable, delete.
  * Les mots séparés par des soulignés (underscore) ou collés avec des majuscules (enDosDeChameau, CamelBumps) sont "découpés" afin d'être prononcés convenablement. Exemple : myObject.getProperty(), my_object.get_name().
  * Le point d'exclamation est utilisé pour la négation, le double esperluette pour le "et" logique (and), le double barre verticale pour le "ou" logique (or), le double égal pour le teste d'égalité entre 2 valeurs, le triple égal pour l'égalité stricte en PHP... la prononciation de symboles et une regexp bien placée permettent d'entendre convenablement : if (!expression), if (!(a && b)), if (!a || !b), if (a >= b)...
  * J'ai mis aussi les noms de fonctions et constantes en langages dérivés du C, les noms de balises HTML, de propriétés CSS. Exemple : sprintf(), ksort(), memcpy(), <title>, <textarea>, background, 1.5em...
  * Liste des langages pleinement supportés : Batch, C, HTML, Java, LaTeX, LibreOffice Math, Lua 4.0, SQL
  * Langagespartiellement supportés : PHP et dérivés du C
* Musique :
  * Je suis musicien, j'utilise des logiciels en anglais et en français, sur des partitions je peux avoir des noms d'instruments dans les 2 langues. J'ai donc ajouté des termes techniques et des noms d'instruments dans le dictionnaire : quarter (une noire), take (une prise), violin (violon), Hohner (une marque d'accordéon), Xfer (nom d'un VST)... ainsi que la prononciation d'instruments du monde : bağlama, banjo, cavaquinho, cheng, çura, marimba...
  * Noms de compositeurs : Wolfgang Amadeus, Beethoven, Schubert, Ligeti...
* Cellules de tableur jusqu'à la colonne ZZ ;
* Anglais : verbes et mots  fréquents ou techniques, verbes irréguliers ;
* Caractères diacrités et spéciaux de l'alphabet latin: prononciation quand isolé, et quelques caractères transformés dans un mots pour langues ibériques, slaves, roumain et nordiques, exemple : España [Espagna], João [Jo-an-o], Dvořák	[Dvorjak], Bregović (Brégovitsh], Kruševo [Krouchévo], Čoček (Tchotchek], Bokmål...
* Noms propres : pays, états américains, régions et villes de France / Allemagne / Grande-Bretagne / USA, et quelques villages imprononçables d'Auvergne ;
* Termes en rapport avec la finance (types de comptes bancaires, brokers, paires Forex, crypto-monnais) ;
* Quelques acronymes administratifs français.

Avant tout, j'ai tenu à ce qu'un texte français soit correctement prononcé. Il y a donc des termes anglais ou techniques qui ne sont pas traités. Par exemple : file (fichier en anglais, et file d'attente), border (bordure en CSS, frontière en anglais, et le verbe border en français). Autre exemple, le verbe try (essayer en anglais) est traité, ainsi que sa forme passée tried, mais pas le nom au pluriel tries, car c'est le verbe trier à la deuxième personne du singulier en français.

Ce dictionnaire m'est utile au quotidien, et le sera pour mon fils qui va être équipé d'un ordinateur au collège, qui va donc apprendre du français, des mathématiques, utiliser Libre Office pour écrire des formules, la chimie, la musique, etc...


## Optimisé pour le synthétiseur IBMTTS
Le synthétiseur IBMTTS, qui n'est pas tout à fait un addon officiel, est elon le moi le plus efficace en terme de temps de réponse, et qui n'apporte pas de reconstitution des acronymes en noms à rallonge comme le font les voix de synthèse de Microsoft.

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
12. Cocher "Se baser sur la langue de la voix pour le traitement des caractères et symboles".

## 
