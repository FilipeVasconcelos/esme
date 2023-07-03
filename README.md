# esme

Templates LaTeX de l'ESME. 

## beamer :

Deux possibilités :
1. copier les fichiers `*.sty` et le dossier `img/` 
   en local avec votre fichier `.tex`

ou 

2. copier le dossier `beamer` dans votre TEXMFHOME (ex.  ~/texmf/tex/latex/ )
   ou le dossier `esme` dans `beamer/themes` si ces derniers existent déjà  

## examen :

Placer `examen.sty` en local ou dans votre installation TEXMFHOME

### Utilisation

Pour chaque examen l'utilisateur doit alors configurer quelques variables 
dans le fichier `.tex` :

```
\newcommand\promo{\texttt{<PROMO>}}                     
\newcommand\module{\texttt{<MODULE>}}                  
\newcommand\annee{\texttt{2022-2023}}                  
\newcommand\epreuve{\texttt{<EPREUVE>}}                
\newcommand\titreEval{\texttt{<TITRE DE L'EVALUATION>}}
\newcommand\dureeEval{\texttt{<X>}}                   
\usepackage{examen}
\reponse{false}
```

1. `promo` : Nom de la promo (ex. IngéSUP, IngéSPE, Ingé1)
2. `module` : Nom du module (ex. Systèmes Techniques, Mathématiques Fondamentales )
3. `annee` : Année scolaire (ex. 2022-2023)
4. `epreuve` : Nom de l'épreuve (ex. Midterm, Final Exam)
5. `titreEval` : Nom de l'évaluation (ex. Dynamique et Déformation, Série Entière)
6. `dureeEval` : Nombre d'heures de l'évaluation (ex. 2)
7. `reponse` : variable spécifiant si le document est un document réponse (ex. `\reponse{true}` ou `\reponse{false}` 
