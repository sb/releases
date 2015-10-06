# Small Basic 1.1 est arrivé!

*Yan Grenier &ndash; 29 March 2015 00:45*

Depuis l'année dernière, nous avons commencé l'aventure du
développement continu de Microsoft Small Basic. Avec une nouvelle
équipe rassemblée au sein de Microsoft dans un nouveau monde
de périphériques et de plateformes.

Comme vous pouvez l'imaginer, nous faisons une étape à la fois.
Cette version est un petit pas, mais c'est une  étape importante.
S'il vous plait rejoignez-nous pour essayer Small Basic 1.1, et
postez vos impressions dans les commentaires ci-dessous.

Nous vous proposons deux possibilités pour télécharger Microsoft
Small Basic:

- Small Basic 1.1 - Si vous êtes sur Windows 7 / Windows Vista ou
  un système plus récent
- Small Basic 1.0 - Si vous êtes sur Windows XP ou un système plus
  ancien
  
  
### Microsoft Small Basic 1.1

Small Basic 1.1 à été mis à niveau vers le Framework NET 4.5, et 
inclus le correctif du bug de l'API Flickr (1.0-17). Il est 
compatible avec Windows 10 Tech Preview, Windows 8.1, Windows 8,
Windows 7, Windows Server 2008 R2, et Windows Vista. Si vous 
utilisez Windows XP, vous devrez télécharger Small Basic 1.0. 
Toutes les extensions créées pour Small Basic 1.0 devrons être 
recompilées pour Small Basic 1.1. Vous avez deux options pour le
téléchargement:

- [Téléchargement Direct en Français][1] - Après le téléchargement,
  exécuter le fichier MSI. Les autres langues sont toujours 
  disponibles dans l'Assistant d'Installation.
- [Page du Centre de Téléchargement][2] - Vous pouvez directement 
  sélectionner et télécharger votre langue depuis cette page. Vous
  y trouverez également des informations sur les nouveautés.
  
Vous trouverez également des informations sur cette version dans 
l'article [Microsoft Small Basic 1.1 Release Notes][3].

[1]: https://www.microsoft.com/fr-FR/download/confirmation.aspx?id=46392
[2]: https://www.microsoft.com/fr-FR/download/details.aspx?id=46392
[3]: http://social.technet.microsoft.com/wiki/contents/articles/30518.microsoft-small-basic-1-1-release-notes-fr-fr.aspx


### Microsoft Small Basic 1.0

Small Basic 1.0 est compatible avec Windows XP, Windows Server 2003
et les systèmes plus anciens. Il nécessite le Framework .NET 3.5 SP1.
Il n'inclus pas le correctif de l'API Flickr du Small Basic 1.1. Vous
avez deux options de téléchargement:

- [Téléchargement Direct en Anglais][4] -  Une fois le fichier MSI
  téléchargé, exécutez le. Les autres langues sont disponibles dans
  l'Assistant d'Installation.
- [Page du Centre de Téléchargement][5] - Vous y trouverez plus 
  d'information sur cette installation (En Anglais uniquement). 
  
[4]: http://download.microsoft.com/download/C/A/F/CAF9E062-94D3-4003-80D9-44CDF7EC7BD9/SmallBasic.msi
[5]: http://www.microsoft.com/en-us/download/details.aspx?id=22961


### Quoi de Neuf dans Microsoft Small Basic 1.1

#### Nouvelles mise à jour

- **Framework NET 4.5** - Nous avons mis à niveau vers le Framework
  .NET de la version 3.5 SP1 vers la version 4.5. Bien que cela provoque
  des ruptures de comportement (voir plus bas), c'était nécessaire afin
  de permettre la création de nouveaux objets tirant parti des nouveaux
  dispositifs, systèmes d'exploitation et capacités.
- **Langues de Téléchargement** - Vous désormais télécharger directement
  Small Basic dans votre langue depuis le Centre de téléchargement. Voir
  la [Page du Centre de Téléchargement][2].
  
  
#### Corrections de Bugs

- **Objet Flickr (1.0-17)** - Flickr à modifié ces API, ce qui à rendu
  inutilisable l'objet Flickr. Ceci a été corrigé dans Small Basic 1.1.
  
  
#### Ruptures avec les précédentes versions

- **Windows XP** - u fait de la mise à niveau vers le Framework .NET 
  4.5, Small Basic 1.1 ne fonctionne pas sur Windows XP et les systèmes 
  plus anciens. Nous continuons de proposer [Small Basic 1.0][6] pour les 
  utilisateurs de Windows XP et de systèmes plus anciens.
- **Extensions 1.0** - Toutes les extensions créées pour Small Basic
  1.0 doivent être recompilées pour Small Basic 1.1 et redistribuées.
  
[6]: http://www.microsoft.com/download/details.aspx?id=22961


#### Autres Modifications

Nous expérimentons des graphismes plus modernes. Actuellement seul 
l'Assistant d'Installation a été modifié avec des graphismes 
modernisés temporaires. Ils seront actualisés à nouveau dans les 
prochaines versions.


### Configuration Système

- **Système d'exploitation pris en charge:**  
  Windows 10 Tech Preview, Windows 8.1, Windows 8, Windows 7, Windows
  Server 2008 R2, Windows Vista, Mini-Mac (Windows 8.1 / Parallels 
  Desktop 10 for Mac / Mac OS X Yosemite), Lifebook (voir les 
  instructions d'installation)
- **Framework .Net 4.5:**  
  Obligatoire pour Windows 7 et Windows Vista. Il est pré-installé 
  sur Windows 8 et les systèmes plus récents.
  
  
### Instructions d'Installation

1. Si vous avez Small Basic 1.0 d'installé, désinstallez-le. Vous 
   devrez également effacer tous les fichiers dans le dossier 
   "smallbasic".
     - A NOTER: Si vous faîtes une installation sur Lifebook (Windows
       8.1 J), vous devrez modifier autoriser l'accès au dossier
       `C:\Users\xxx\AppData\Roaming\Microsoft` à `SYSTEM`.
2. Télécharger et Installer Microsoft Small Basic dans votre langue
   préférée.
3. Lancer Microsoft Small Basic en cliquant sur le raccourci de son
   programme.
   
Merci de vous joindre à nous dans notre aventure Small Basic. Nous
avons parcouru un long chemin, mais comme vous pouvez le constater,
nous venons seulement de commencer ! 

"Small basic" quement votre,

Yan