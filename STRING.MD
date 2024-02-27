## Guide Complet pour la Manipulation des Chaînes de Caractères en Python

### Création
- Créer une chaîne de caractères : `s = "Bonjour, le monde!"`

### Concaténation
- Concaténer des chaînes de caractères : `s + " Au revoir."`

### Slicing (Découpage)
- Extraire une sous-chaîne : `s[1:5]` extrait les caractères de l'index 1 à 4.
- Extraire du début jusqu'à un index : `s[:5]` extrait les 5 premiers caractères.
- Extraire d'un index jusqu'à la fin : `s[6:]` extrait tout depuis l'index 6.
- Accéder au dernier caractère : `s[-1]`

### Autres Opérations Utiles

#### Vérification de Contenu
- Vérifier si une chaîne contient une sous-chaîne : `"monde" in s`
- Vérifier si une chaîne ne contient pas une sous-chaîne : `"monde" not in s`

#### Itération
- Itérer à travers chaque caractère : `for char in s:`

#### Longueur de la Chaîne
- Obtenir la longueur d'une chaîne : `len(s)`

#### Comparaison de Chaînes
- Comparer l'égalité : `s == "une autre chaîne"`
- Comparer les différences : `s != "une autre chaîne"`

#### Conversion de Nombres en Chaînes et Vice Versa
- Convertir un nombre en chaîne : `str(10)`
- Convertir une chaîne en un nombre entier : `int("10")`
- Convertir une chaîne en un nombre à virgule : `float("10.01")`

### Formatage
- Formater les chaînes en utilisant `format()` : `"Mon nom est {}.".format("Jean")`
- Formater en utilisant les f-strings (Python 3.6+) : `f"Mon nom est {nom}."`

### Caractères d'Échappement
- Utiliser des caractères d'échappement pour inclure des caractères spéciaux : `s = "Il a dit, \"Bonjour!\""`

### Chaînes Multilignes
- Créer des chaînes sur plusieurs lignes en utilisant des triples guillemets : 
  ```python
  s = """Ceci est un exemple
  de chaîne sur plusieurs lignes.
  Parfait pour des commentaires longs ou de la documentation."""


## Méthodes Fréquentes pour les Chaînes de Caractères (`str`) en Python

### Manipulation Générale
- `capitalize()`: Met en majuscule la première lettre de la chaîne.
- `title()`: Met en majuscule la première lettre de chaque mot.
- `upper()`: Convertit toutes les lettres en majuscules.
- `lower()`: Convertit toutes les lettres en minuscules.
- `swapcase()`: Inverse la casse de toutes les lettres de la chaîne.

### Recherche et Remplacement
- `count(sub[, start[, end]])`: Compte combien de fois le sous-chaîne `sub` apparaît dans la chaîne.
- `startswith(prefix[, start[, end]])`: Vérifie si la chaîne commence par le `prefix`.
- `endswith(suffix[, start[, end]])`: Vérifie si la chaîne se termine par le `suffix`.
- `find(sub[, start[, end]])`: Recherche `sub` et retourne l'indice le plus bas où la sous-chaîne est trouvée.
- `rfind(sub[, start[, end]])`: Semblable à `find`, mais recherche de la fin.
- `index(sub[, start[, end]])`: Semblable à `find`, mais lève une `ValueError` si `sub` n'est pas trouvé.
- `rindex(sub[, start[, end]])`: Semblable à `index`, mais recherche de la fin.
- `replace(old, new[, count])`: Remplace toutes les occurrences de la sous-chaîne `old` par `new`.

### Suppression d'Espaces
- `strip([chars])`: Supprime les espaces (ou autres caractères spécifiés) au début et à la fin.
- `lstrip([chars])`: Supprime les espaces au début.
- `rstrip([chars])`: Supprime les espaces à la fin.

### Séparation et Jointure
- `split(sep=None, maxsplit=-1)`: Divise la chaîne à chaque occurrence de `sep` et retourne une liste.
- `rsplit(sep=None, maxsplit=-1)`: Semblable à `split`, mais divise de la fin.
- `splitlines([keepends])`: Divise la chaîne aux sauts de ligne et retourne une liste de lignes.

### Autres Méthodes Utiles
- `join(iterable)`: Joint les éléments d'un itérable pour former une chaîne.
- `zfill(width)`: Ajoute des zéros à gauche de la chaîne, jusqu'à ce que la largeur spécifiée soit atteinte.
- `center(width[, fillchar])`: Centre la chaîne dans une chaîne de largeur `width`.
- `ljust(width[, fillchar])`: Justifie la chaîne à gauche dans une chaîne de largeur `width`.
- `rjust(width[, fillchar])`: Justifie la chaîne à droite dans une chaîne de largeur `width`.
- `encode(encoding="utf-8", errors="strict")`: Encode la chaîne en utilisant l'encodage spécifié.
- `format(*args, **kwargs)`: Formate la chaîne.
- `format_map(mapping)`: Formate la chaîne en utilisant un dictionnaire.


