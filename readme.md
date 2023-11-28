---
title: Base de donné la FLAC
---

# Présentation

Cette API a été conçue à partir de Strapi. Elle permet de gérer une base
de donné avec des produits, et des catégories.

Cette base fonctionne sur le principes de routes à faire avec des fetch.

# Démarrer

## Récupérer l'API

Copier la ligne suivante pour récuparer l'API dans votre terminal :

```bash
git clone <git@github.com:theotime2005/salezy>
```

## Installer les dépendances

Entrez les lignes suivantes pour installer les dépendances
```bash
cd salezy/backend
npm install
```

# Utilisation
# Lancer et accéder à l'API

Vous pouvez lancer l'API de plusieurs manières :

-   En mode développement : ```bash npm run develop```

-   En mode normal : ```bash npm start```

Pour vous connecter à l'interface d'administration, rendez-vous sur la
page suivante :

```http
http://localhos:1336/admin
```

Email : admin@lesmeilleurs.com
Mot de passe : Administration08

## Accès aux données

L'API fonctionne avec des routes. Par exemples, vous pouvez utiliser la
requête suivante pour récupérer tous les produits :

```http
http://localhost:1337/api/products
```

Certaines requêtes nécessitent une autorisation, soit un token. Par
exemple, dans un fetch, vous pourez utiliser le token de cette manière :

```http
http://localhost:1337/api/categories

Autorisation: Bearer \<votre_token\>
```

Pour obtenir un token, authentifiez-vous via une requête POST.
