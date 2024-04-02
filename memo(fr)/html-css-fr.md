## HTML
## Structure de base

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Titre du document</title>
</head>
<body>

<header>
    <h1>Titre principal</h1>
    <nav>
        <ul>
            <li><a href="#section1">Section 1</a></li>
            <li><a href="#section2">Section 2</a></li>
            <li><a href="#section3">Section 3</a></li>
        </ul>
    </nav>
</header>

<section id="section1">
    <h2>Section 1</h2>
    <p>Contenu ici.</p>
</section>

<section id="section2">
    <h2>Section 2</h2>
    <p>Contenu ici.</p>
</section>

<section id="section3">
    <h2>Section 3</h2>
    <p>Contenu ici.</p>
</section>

<footer>
    <p>&copy; Année | Contenu du pied de page</p>
</footer>

</body>
</html>
```
## Balises HTML courantes

- `<h1>` - `<h6>`: Titres
- `<p>`: Paragraphe
- `<a>`: Ancre (Lien)
- `<img>`: Image
- `<div>`: Division
- `<span>`: Division en ligne
- `<ul>`: Liste non ordonnée
- `<ol>`: Liste ordonnée
- `<li>`: Élément de liste
- `<table>`: Tableau
- `<tr>`: Ligne de tableau
- `<td>`: Donnée de tableau
- `<form>`: Formulaire
- `<input>`: Entrée
- `<textarea>`: Zone de texte

## Attributs HTML courants

- `id`: Identifiant unique
- `class`: Nom de classe pour le style
- `href`: Référence de l'hyperlien
- `src`: Source (par exemple, pour les images)
- `alt`: Texte alternatif pour les images
- `title`: Texte d'infobulle

## Éléments de formulaire

```html
<form>
    <label for="name">Nom :</label>
    <input type="text" id="name" name="name" required>
    <br>
    <label for="email">Email :</label>
    <input type="email" id="email" name="email" required>
    <br>
    <input type="submit" value="Soumettre">
</form>
```