```md
# Facebook SignUp Page – Clone HTML & CSS

Ce projet est une reproduction de la page d’inscription de Facebook réalisée uniquement avec **HTML et CSS**, dans un objectif pédagogique.  
Il met l’accent sur la **structure sémantique**, l’**accessibilité**, le **design moderne** et le **responsive design**.

## Aperçu du projet

Cette interface permet à un utilisateur de :
- Renseigner son **prénom et nom**
- Entrer son **email ou numéro**
- Créer un **mot de passe**
- Sélectionner sa **date de naissance**
- Choisir son **genre**
- Consulter les **mentions légales**

## Objectifs pédagogiques

- ✅ Reproduire une interface réaliste  
- ✅ Maîtriser les bases solides en **HTML & CSS**  
- ✅ Appliquer les règles d’**accessibilité web**  
- ✅ Comprendre la **logique des formulaires**  
- ✅ Créer un design **responsive**  
- ✅ Développer l’**attention au détail**  
- ✅ Se préparer à l’**intégration front-end professionnelle**

## Spécifications techniques

- ✔️ Respect du **style guide**
- ✔️ Structure **HTML sémantique**
- ✔️ Formulaire **complet et accessible**
- ✔️ Design **responsive**
- ✔️ Code **propre et maintenable**
- ✔️ Aucune dépendance externe

## Technologies utilisées

- ✅ HTML5  
- ✅ CSS3  
- ❌ Aucun framework  
- ❌ Aucun JavaScript  
- ❌ Aucune bibliothèque externe

## Structure du projet

```

📁 dos
┣ 📄 index.html   → Structure de la page
┣ 📄 index.css    → Design et responsive
┗ 📄 README.md    → Documentation
┗ 🖼️ Capture d'écran → Capture d'ecran pour le projet


````

# Explication du Code

## 1️⃣ Le fichier `index.html`

### Structure principale

```html
<div class="container">
  <header>...</header>
  <main>...</main>
</div>
````

* `container` : centre toute la page
* `header` : contient le logo Facebook et le slogan
* `main` : contient la carte du formulaire

### Le formulaire

```html
<form id="signup-form">
```

Ce formulaire contient :

* Deux champs pour le **nom** :

```html
<input type="text" id="firstname">
<input type="text" id="lastname">
```

* Un champ pour l’**email ou numéro**

```html
<input type="email" id="email">
```

* Un champ pour le **mot de passe**

```html
<input type="password" id="password">
```

### Date de naissance

```html
<select id="day"></select>
<select id="month"></select>
<select id="year"></select>
```

Trois menus déroulants :

* Jour
* Mois
* Année

Chaque select possède un `aria-label` pour l’accessibilité.

### Genre (Radio Buttons)

```html
<input type="radio" name="gender" value="female">
<input type="radio" name="gender" value="male">
<input type="radio" name="gender" value="custom">
```

Un seul choix possible grâce au même `name="gender"`.

### Bouton d’inscription

```html
<button type="submit" class="signup-button">S'inscrire</button>
```

Envoie le formulaire (même si aucun traitement backend n’est encore lié).

## 2️⃣ Le fichier `style.css`

### Reset CSS

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

Permet d’avoir un affichage propre et identique sur tous les navigateurs.

### Style général

```css
body {
  background-color: #e9ebee;
  color: #1c1e21;
}
```

Reprend les couleurs officielles de Facebook.

### Carte du formulaire

```css
.card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.08);
}
```

Crée l’effet de carte flottante.

### Champs de formulaire

```css
input {
  border: 1px solid #dddfe2;
  background-color: #f5f6f7;
}
```

Style propre et moderne des champs.

### Bouton d’inscription

```css
.signup-button {
  background-color: #42b72a;
}
.signup-button:hover {
  background-color: #36a420;
}
```

Effet de survol pour améliorer l’expérience utilisateur.

### Responsive design

```css
@media (max-width: 768px)
```

* Les champs passent en **colonne**
* Les blocs deviennent plus **larges**
* L’interface reste fluide sur téléphone

## Lancer le projet

```bash
git clone https://github.com/ton-username/ton-repo.git
```

## Accessibilité

* Labels bien associés aux champs
* Attributs `aria`
* Champs obligatoires `required`
* Navigation clavier possible
* Bon contraste visuel

## Auteur

**Boureima Issa Adamou Razak**

# Capture d'écran du Projet 
## Capture d'écran_1024px
![Aperçu de l’interface](Capture d'écran_1024px.png)

## Capture d'écran_768pxpx
![Aperçu de l’interface](Capture d'écran_768px.png)

## Capture d'écran_320px
![Aperçu de l’interface](Capture d'écran_320px.png)
