# Gestion des Factures en Auto-Entrepreneur avec LaTeX

Ce projet permet de générer rapidement des factures personnalisées en utilisant LaTeX. Suivez les étapes ci-dessous pour personnaliser et générer vos factures.

## Prérequis

### Sur Linux et sur Windows via WSL

1. **Installez LaTeX et les paquets nécessaires** :
   - Vous devez installer `pdflatex` (inclus dans le paquet `texlive`) ainsi que quelques paquets supplémentaires pour garantir le bon fonctionnement.
   - Pour installer LaTeX sur une distribution Linux (comme Ubuntu/Debian), exécutez la commande suivante :
     ```bash
     sudo apt update
     sudo apt install texlive-latex-base texlive-science texlive-latex-extra texlive-lang-french
     ```

2. **Autres paquets utiles** :
   - Vous pourriez également avoir besoin de `make` pour la gestion de la compilation des fichiers `.tex` :
     ```bash
     sudo apt install make
     ```

## Utilisation
- Commencer par editer le fichier .input/facture_footer.tex pour le personaliser
- Renommer/Copier le fichier FA201201-001.tex et y modifier le client et ajouter des lignes de facturation
- tapez "make"
    - "make world" va compiler les pdf en laissant les aux et log de latex
    - "make FA201201-001.pdf" va compiler le pdf cite a partir du .tex correspondant
    - "make clean" va retirer les aux et log de latex
    - "make flush" va effacer les pdf
    - "make all"/"make" va compiler les pdf et effacer les aux et log

## Sources
- http://i.got.nothing.to/hack/on/gestion-des-factures-en-autoentrepreneur/
- http://godefroy.me/latex-comment-faire-rapidement-une-facture-super-classe-a530591
- https://blog.tengu.ch/blog/post/47
