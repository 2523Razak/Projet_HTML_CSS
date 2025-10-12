# Exerce_1 – Grille de prix simple en HTML & CSS

## Description du projet

Ce projet est une **page web simple** qui présente une grille de prix pour un service ou un abonnement.
Il est conçu pour que les débutants en HTML et CSS puissent comprendre comment structurer une page, styliser des éléments et créer une mise en page responsive (qui s’adapte aux écrans d’ordinateur et de téléphone).

## Contenu du projet

Le projet contient deux fichiers principaux :

* `index.html` → Contient tout le contenu visible sur la page
* `index.css` → Contient les styles pour rendre la page jolie et lisible

## Explication du code HTML

### 1. Déclaration du document et en-tête

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grille de prix simple</title>
    <link rel="stylesheet" href="index.css">
</head>
```

* `<!DOCTYPE html>` : Indique que c’est un document HTML5.
* `<html lang="fr">` : Définit la langue du site en français.
* `<meta charset="UTF-8">` : Permet d’afficher correctement les accents.
* `<meta name="viewport"...>` : Rend la page responsive sur mobile.
* `<link rel="stylesheet" href="index.css">` : Relie le CSS pour le style.

### 2. Corps de la page (`<body>`)

```html
<body>
    <div class="boite-principale">
        ...
    </div>
</body>
```

* `<body>` contient tout ce qui sera visible sur la page.
* `<div class="boite-principale">` est le conteneur principal qui regroupe tout le contenu.

### 3. En-tête visible

```html
<section class="entete">
    <h2>Rejoins notre groupe</h2>
    <p class="garantie">Garantie 30 jours satisfait ou remboursé</p>
    <p>Accède à tous nos tutoriels faits par des pros...</p>
</section>
```

* `<section>` : Groupe logique d’éléments.
* `<h2>` : Titre principal de la section.
* `<p>` : Paragraphe pour les textes explicatifs.
* `.garantie` : Classe CSS utilisée pour styliser le texte de garantie.

### 4. Section des prix et avantages

```html
<div class="section-prix">
    <section class="abonnement">
        ...
    </section>
    <section class="avantages">
        ...
    </section>
</div>
```

* Contient deux blocs côte à côte :

  1. **Abonnement** → Prix et bouton pour s’inscrire
  2. **Avantages** → Liste des bénéfices pour l’utilisateur

## Explication du code CSS

### 1. Réinitialisation des marges et paddings

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

* Supprime les marges et paddings par défaut pour tous les éléments, ce qui facilite le contrôle du design.

### 2. Style du corps de la page

```css
body {
    font-family: Arial, sans-serif;
    background-color: #eaf3f7;
    color: #333;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
}
```

* Police, couleur, fond et centrage de la page.
* `display: flex; justify-content: center; align-items: center;` → Centre le contenu horizontalement et verticalement.

### 3. Boîte principale

```css
.boite-principale {
    max-width: 650px;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    overflow: hidden;
}
```

* Délimite la zone principale et ajoute des coins arrondis et une ombre.

### 4. En-tête

```css
.entete { background-color: #fff; padding: 30px; }
.entete h2 { color: #1eb8a8; margin-bottom: 20px; font-size: 1.5rem; }
.garantie { color: hsl(71, 73%, 54%); font-weight: bold; margin-bottom: 15px; }
```

* Styles pour les titres et le texte de la garantie.

### 5. Section des prix et avantages

```css
.section-prix { display: flex; flex-wrap: wrap; }
.abonnement, .avantages { flex: 1; min-width: 300px; padding: 30px; }
```

* Utilise Flexbox pour mettre les deux blocs côte à côte.
* `flex-wrap: wrap` permet aux blocs de se placer en colonne sur mobile.

### 6. Styles spécifiques

* **Abonnement** : fond coloré, texte blanc, prix en gros, bouton interactif.
* **Avantages** : fond différent, liste sans puces par défaut, éléments espacés.

### 7. Responsive (mobile)

```css
@media (max-width: 768px) {
    .section-prix { flex-direction: column; }
}
```

* Sur les écrans petits, les deux blocs passent l’un en dessous de l’autre pour mieux s’afficher.

## Objectifs pédagogiques

1. Comprendre la structure d’une page HTML.
2. Apprendre à styliser avec CSS : couleurs, polices, marges, Flexbox.
3. Découvrir comment rendre un site responsive.
4. Pouvoir reproduire la grille de prix pour vos propres projets.
