# Confirmation de Présence en Ligne

Ce projet est une page web permettant aux participants de confirmer leur présence en ligne pour un cours. Elle inclut également des fonctionnalités pour que l'administrateur puisse accéder aux enregistrements des participants et télécharger les fichiers du cours.

## Fonctionnalités

1. **Formulaire de confirmation de présence** :
   - Les participants peuvent fournir les informations suivantes :
     - Nom
     - Post-nom
     - Prénom
     - Promotion (L1, L2, L3)
     - Faculté (BA, SPA, CTI, Théologie)
     - Vacation (Matin, Soir)
     - Heure de connexion
     - Heure de déconnexion
     - Titre du cours
   - Un message de confirmation est affiché après la soumission.

2. **Gestion des enregistrements :
   - Une section réservée à l'administrateur contient les fichiers téléchargeables (par exemple, des fichiers PDF liés au cours).
   - Accessible uniquement avec un mot de passe administrateur.

3. **Responsive Design** :
   - La page s’adapte aux différents types d’écrans (ordinateur, tablette, smartphone).

## Structure des fichiers

- `index.html` : Page principale contenant le code HTML, CSS et JavaScript.
- `logo-universite.png` : Fichier image pour le logo de l’université (remplacer par votre propre logo).
- `cours1.pdf`, `cours2.pdf` : Exemple de fichiers de cours téléchargeables (à remplacer par vos fichiers).

## Configuration

1. **Changement du logo** :
   - Remplacez le fichier `logo-universite.png` par le logo de votre université.
   - Assurez-vous que le nom et le chemin du fichier sont corrects dans le code HTML : `<img src="logo-universite.png" alt="Logo de l'université">`.

2. **Ajout de fichiers de cours** :
   - Placez vos fichiers PDF ou autres documents dans le même dossier que le fichier HTML.
   - Ajoutez-les dans la section administrateur (dans le div avec la classe `file-list`) :
     ```html
     <a href="nom-du-fichier.pdf" download>Télécharger le fichier</a>
     ```

3. **Mot de passe administrateur** :
   - Par défaut, le mot de passe pour accéder à la section administrateur est `admin123`.
   - Vous pouvez le modifier dans le script JavaScript (ligne où `adminPassword` est défini) :
     ```javascript
     const adminPassword = "votre-mot-de-passe";
     ```

## Hébergement

### Méthodes recommandées :
1. **Netlify** :
   - Téléversez les fichiers sur [Netlify](https://www.netlify.com).
   - Obtenez une URL publique gratuitement.

2. **GitHub Pages** :
   - Créez un repository sur [GitHub](https://github.com).
   - Téléversez vos fichiers dans le repository.
   - Activez GitHub Pages depuis les paramètres pour héberger votre site gratuitement.

3. **Autres hébergeurs** :
   - Utilisez un hébergement classique (comme OVH, Hostinger ou Bluehost) en téléversant les fichiers via FTP.

## Utilisation

1. **Participant** :
   - Remplissez les champs du formulaire (Nom, Post-nom, Prénom, etc.).
   - Cliquez sur le bouton **Confirmer ma présence**.
   - Un message de confirmation s’affichera.

2. **Administrateur** :
   - Entrez le mot de passe administrateur dans la boîte de dialogue qui s’affiche au chargement de la page.
   - Si le mot de passe est correct, la section contenant les fichiers téléchargeables sera visible.

## Aperçu

### Formulaire de présence :
![Formulaire](https://via.placeholder.com/800x400?text=Apercu+du+formulaire)

### Section administrateur :
![Section Admin](https://via.placeholder.com/800x400?text=Apercu+section+admin)

## Licence

Ce projet est libre d'utilisation et peut être modifié selon vos besoins. Aucune attribution n'est requise.
