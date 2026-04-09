 # Nexus Compiler:
Un compilateur C interactif, simple et autonome, pour Windows, inspiré des outils CLI classiques. c'est le compileur fichier.c --> fichier.exe le plus simple d'utilisation.

 Fonctionnalités:
Interface CLI intuitive : Commandes simples, comme un terminal de développement

Éditeur intégré : Ouvre/modifie des fichiers .c directement avec nano <fichier> (utilise Bloc-notes Windows)
Compilation C en un clic : Compile des fichiers source avec make <src> <exe> (utilise le GCC de Dev-C++ installé sur le système)
Suppression de fichiers : Supprime des fichiers directement depuis le terminal avec rm <fichier>
Sans dépendances externes : Pas besoin de copier gcc.exe, DLLs ou fichiers supplémentaires dans le dossier
Anti-récursivité : Empêche la compilation de l'EXE lui-même (évite les erreurs de permission Windows)
Copyright 2026 : Mise à jour pour l'année en cours
 
 Prérequis:
Windows 10/11
Dev-C++ (ou MinGW-w64) installé sur votre système (pour avoir accès à gcc.exe dans le PATH système)
Aucun autre logiciel requis
 Installation & Utilisation
1. Compilation du projet
Ouvrez le fichier nexus_compiler.c dans Dev-C++
Compilez le code (F11) pour générer l'exécutable nexus_compiler.exe
Placez l'exécutable dans n'importe quel dossier de votre choix
2. Utilisation
Lancez nexus_compiler.exe et utilisez les commandes suivantes :

Commande	Description
nano <fichier>	Ouvre le fichier avec Bloc-notes (crée le fichier s'il n'existe pas)
make <src> <exe>	Compile le fichier source <src>.c en un exécutable <exe>.exe
rm <fichier>	Supprime le fichier spécifié (sans passer par l'explorateur Windows)
help / h	Affiche la liste des commandes disponibles
exit / quit	Quitte le programme
Exemple d'utilisation:
bash：

 Créer un fichier test.c
nexus> nano test.c
 (Écrivez votre code C dans Bloc-notes, enregistrez et fermez)

Compiler le fichier en test.exe
nexus> make test test
[+] Compilation...
[✓] SUCCES : test.exe cree

 Supprimer l'exécutable
nexus> rm test.exe
[✓] Fichier supprime : test.exe

 Quitter
nexus> exit

 Dépannage
Erreur Permission denied
Cause : Vous essayez de compiler l'EXE de Nexus lui-même (nexus.c) pendant qu'il est en cours d'exécution
Solution : Fermez nexus_compiler.exe, recompilez le code dans Dev-C++, puis relancez-le
Erreur gcc: command not found
Cause : Dev-C++/MinGW n'est pas installé, ou gcc.exe n'est pas dans le PATH système
Solution : Installez Dev-C++ (disponible gratuitement sur 
SourceForge
File
) et assurez-vous que l'option "Add MinGW to PATH" est cochée lors de l'installation
Erreur CreateProcess: No such file or directory
Cause : Tentative d'utilisation de gcc.exe externe sans tous les fichiers MinGW
Solution : Utilisez la version système de GCC (intégrée à Dev-C++), pas de copie de fichier nécessaire

comment utiliser:
mettez le dans un dossier avec gcc.exe et tous les autres fichier neccecaire a son fonctionnement.
ouvrez et vous pouvez taper help pour avoir une aide.

 Licence:
Ce projet est open-source, sous licence MIT.
© 2026 NDG Dev Team. Tous droits réservés.

Contribution:
Les contributions sont les bienvenues ! N'hésitez pas à ouvrir des issues ou des pull requests pour améliorer le projet.

 Contact:
Pour toute question ou suggestion, contactez l'équipe NDG Dev Team. E-mail: yyley2025@hotmail.com  merci de bien vouloir denoncer tous problemes.

 Pourquoi ce projet ?
Nexus Compiler a été créé pour offrir un outil de compilation C simple, accessible et autonome, pour les débutants comme pour les développeurs, sans les complications des outils complexes.
Note : Ce projet utilise le compilateur GCC de Dev-C++/MinGW, qui est un logiciel open-source gratuit.


Notez nexus compiler avec yyley2025@hotmail.com

MERCI DE VOTRE UTILISATION 

L'EQUIPE NCDG

# TOUT LE PROJET A ETE CREE PAR L'EQUIPE DU NCDG, CONTENANT 1 PERSONNE. MERCI POUR VORE SOUTIEN.




