# Mise en ligne GitHub

## Nom recommandé

`Lux-Kybernetica/NAG_HAMMADI_LIBRARY_FR`

Alternative si vous voulez insister sur la notion de snapshot :

`Lux-Kybernetica/NAG_HAMMADI_PUBLIC_RELEASE`

## Description GitHub

> Corpus français de recherche de la bibliothèque de Nag Hammadi : 45 œuvres, 6 670 segments alignés, provenance et validation structurelle.

## Visibilité

**Public**

## Topics recommandés

```text
nag-hammadi
gnosticism
coptic
digital-humanities
ancient-texts
french-translation
corpus
textual-scholarship
rag
lux-kybernetica
```

## Site

`https://luxkybernetica.org`

## Étapes

1. Créer le repository dans l’organisation **Lux-Kybernetica**.
2. Le rendre **Public**.
3. Ne pas ajouter de README ou de licence lors de la création si vous comptez pousser ce dossier tel quel.
4. Extraire le ZIP du kit.
5. Ouvrir PowerShell dans le dossier extrait.

Puis :

```powershell
git init
git add .
git commit -m "release: publish French Nag Hammadi research corpus v0.1.0"
git branch -M main
git remote add origin https://github.com/Lux-Kybernetica/NAG_HAMMADI_LIBRARY_FR.git
git push -u origin main
```

Si vous choisissez le nom `NAG_HAMMADI_PUBLIC_RELEASE`, remplacez simplement l’URL du remote.

## Avant le push final

Décider la licence de la couche française et ajouter le fichier `LICENSE`.

Recommandation actuelle : **CC BY 4.0** si l’objectif principal est l’accès et la réutilisation.
