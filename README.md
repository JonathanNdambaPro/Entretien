# Entretien technique

Ce repo a pour objectif de tester vos compétences en software et data engineering. Cet entretien n’a aucune limite de temps et vous pouvez vous aider de n’importe quel outil (IA incluse).

Vous devez être en mesure de justifier vos choix de design et/ou architecturaux, en indiquant leurs avantages et leurs limites lors de notre entretien vidéo.

Vous n’êtes pas obligé·e de résoudre tous les exercices ; faites simplement de votre mieux.

## Exercices : Software Design

**Attention :** consultez le dossier `entretien_technique`  pour cette section.

### Exercice 0

Installer [uv](https://docs.astral.sh/uv/guides/install-python/) et tout ce dont vous avec besoin dans le `Makefile`

### Exercice 1

Dans le sous-dossier `entretien_technique`, plusieurs scripts ne sont pas optimaux car ils sont difficiles à maintenir et à faire évoluer. Refactorisez-les.

### Exercice 2

Mettez en place des tests avec pytest pour le code (refactorisé ou non si vous n’y êtes pas parvenu) afin d’obtenir une couverture minimale de 80 %.

### Exercice 3

Ajoutez des docstrings au format NumPy dans le code.  
**Bonus :** configurez mkdocs pour qu’il génère la documentation à partir des docstrings.

## Exercices : Git

L’historique Git de ce projet contient trop de commits. Veillez à n’en conserver que deux :  

- le premier, `a1bafdb feat: init`
- un second, que vous nommerez comme vous le souhaitez, mais dont le message devra respecter la convention [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

## Exercices : Data Modeling

### Exercice 1 : Normalisation

Normalisez la table suivante en 3NF :

| ÉtudiantID | Nom    | CoursInscrits           | DeptID | NomDept  |
| ---------- | ------ | ----------------------- | ------ | -------- |
| S01        | Alice  | Mathématiques; Physique | D01    | Sciences |
| S02        | Bob    | Histoire                | D02    | Lettres  |
| S03        | Carole | Physique; Informatique  | D01    | Sciences |
| S04        | David  |                         | D03    | Droit    |

### Exercice 2 : Modélisation dimensionnelle

Faites une modélisation en étoile pour cette table :

| vente\_id | date\_vente | client\_id | nom\_client | segment\_client | produit\_id | designation     | categorie    | prix\_unitaire | quantite |
| --------- | ----------- | ---------- | ----------- | --------------- | ----------- | --------------- | ------------ | -------------- | -------- |
| 1001      | 2025-06-15  | C100       | Dupont      | Standard        | P100        | Smartphone X    | Électronique | 299,00         | 2        |
| 1002      | 2025-07-01  | C100       | Dupont      | Premium         | P200        | Coque Téléphone | Accessoire   | 19,00          | 1        |
| 1003      | 2025-07-12  | C101       | Martin      | Standard        | P100        | Smartphone X    | Électronique | 299,00         | 1        |
| 1004      | 2025-07-20  | C100       | Dupont      | Premium         | P100        | Smartphone X    | Électronique | 299,00         | 1        |

## Exercice : System design/Data Architecture

Concevez une architecture de données sur GCP en vous appuyant uniquement sur des outils open source pour des traitements batch. Vous pouvez la réaliser sur [Excalidraw](https://excalidraw.com/).
