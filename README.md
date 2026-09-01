# Nag Hammadi Library — Corpus français de recherche

**45 œuvres distinctes · 6 670 segments alignés · Lux Kybernetica · 2026**

> Une édition numérique française de recherche de la bibliothèque de Nag Hammadi, conçue comme un corpus **traçable, segmenté, versionné et interrogeable**.

## État du corpus

| Couche | État |
|---|---|
| 45 œuvres distinctes identifiables | ✅ Complètes |
| Traduction française de recherche | ✅ 45 / 45 |
| Segments alignés | ✅ 6 670 |
| Validation structurelle globale | ✅ PASS |
| Erreurs structurelles connues | ✅ 0 |
| Warnings structurels non adjudiqués | ✅ 0 |
| Exceptions éditoriales documentées | 19 |
| Revue sémantique exhaustive | 🟡 En cours |
| Adjudication philologique directe contre le copte | 🟡 À poursuivre |
| Séparation stricte de tous les témoins manuscrits | 🟡 Partielle |

## Pourquoi ce dépôt existe

Nag Hammadi est déjà disponible dans plusieurs éditions et traductions savantes. Ce dépôt ne prétend donc ni « découvrir » ces textes, ni remplacer les éditions critiques réalisées directement à partir du copte.

Son objectif est différent : transformer les textes en un **corpus numérique de recherche** dans lequel chaque passage peut être retrouvé, comparé et cité de manière stable.

Chaque fichier de traduction conserve notamment :

- un identifiant d’œuvre et de témoin ;
- la provenance de la traduction anglaise intermédiaire ;
- le SHA-256 du fichier source utilisé au moment de la traduction ;
- des identifiants `SOURCE-ID` et `TARGET-ID` stables ;
- le texte anglais de référence dans des commentaires documentaires ;
- la traduction française correspondante ;
- les marqueurs de pages du codex lorsque la source les fournit ;
- les lacunes, restitutions et corrections éditoriales.

L’objectif à long terme est qu’une affirmation puisse suivre la chaîne :

`question → passage → œuvre → témoin → source → traduction → provenance`

## Méthode de traduction

La couche française est une **traduction de recherche réalisée via des traductions anglaises intermédiaires documentées**.

Elle **n’est pas présentée comme une traduction critique directe du copte**.

Le corpus anglais utilisé repose principalement sur les traductions de **Samuel Zinner**, éditées par **Mark M. Mattison**, publiées par le projet Luminescence / Other Gospels avec un statut de réutilisation documenté comme domaine public.

Voir : [`docs/METHODOLOGY.md`](docs/METHODOLOGY.md) et [`docs/RIGHTS_AND_PROVENANCE.md`](docs/RIGHTS_AND_PROVENANCE.md).

## Signaux éditoriaux conservés

La traduction cherche à préserver la géométrie documentaire du texte source :

- `[ ... ]` : texte restitué / supplied text ;
- `< ... >` : correction éditoriale ;
- `( ... )` : parenthèse éditoriale présente dans la source ;
- marqueurs de lacunes et ellipses ;
- marqueurs et liens de pages des codices ;
- notes et divisions internes.

Dans certains cas, l’ordre des mots français impose de scinder une restitution en plusieurs groupes. Ces écarts sont suivis explicitement au lieu d’être masqués.

## Contenu du dépôt

```text
translations/
    45 fichiers Markdown de traduction française

docs/
    CORPUS_INDEX.md
    METHODOLOGY.md
    RIGHTS_AND_PROVENANCE.md
    STATUS_AND_LIMITATIONS.md
    CITATION.md

.github/
    ISSUE_TEMPLATE/
        translation-correction.yml

README.md
CONTRIBUTING.md
CITATION.cff
RELEASE_NOTES.md
LICENSING.md
GITHUB_SETUP.md
```

## Lire les textes

➡️ [`translations/`](translations/)

➡️ [Index complet des 45 œuvres](docs/CORPUS_INDEX.md)

Les fichiers sont du Markdown UTF-8 et peuvent être lus directement dans GitHub, téléchargés individuellement ou traités comme corpus par des scripts, moteurs de recherche ou systèmes RAG.

## Statut éditorial

**Traduction complète** ne signifie pas **édition critique définitive**.

Le rail de traduction est fermé au niveau des 45 œuvres et la validation structurelle est acquise. Une revue contradictoire a cependant confirmé que la couche sémantique et philologique doit continuer à être améliorée.

Les corrections sont donc bienvenues lorsqu’elles sont accompagnées d’une justification précise et d’un identifiant de segment.

Voir [`CONTRIBUTING.md`](CONTRIBUTING.md).

## RAG et humanités numériques

Le corpus a été conçu pour permettre :

- recherche lexicale ;
- recherche sémantique ;
- concordances ;
- comparaison intertextuelle ;
- cartographie d’entités et de concepts ;
- comparaison de témoins ;
- interrogation RAG avec provenance ;
- intégration future à des systèmes de recherche et de simulation de corpus plus larges.

La priorité est de conserver la preuve documentaire : une réponse générée doit pouvoir remonter à ses passages sources.

## Droits et provenance

Les textes anglais redistribués dans les fichiers de traduction proviennent de sources dont le statut de réutilisation est documenté dans le projet de recherche amont.

Les éditions savantes modernes protégées ne font pas partie de cette publication simplement parce qu’elles ont servi de références bibliographiques.

La licence de la **couche française Lux Kybernetica** doit être explicitement choisie avant de déclarer une licence ouverte. Voir [`LICENSING.md`](LICENSING.md).

## Citer ce corpus

Voir [`docs/CITATION.md`](docs/CITATION.md) ou le fichier [`CITATION.cff`](CITATION.cff).

## Version

**Public Research Corpus v0.1.0 — 2026-09-01**

Ce dépôt est une publication versionnée et évolutive. Les corrections futures doivent préserver l’historique des choix éditoriaux.

---

### English summary

This repository contains a complete **French research-translation layer for 45 distinct Nag Hammadi works**, aligned across **6,670 segments**. The French text is derived from documented English intermediary translations and is **not claimed as a direct critical translation from Coptic**. The corpus is designed for traceable digital research, semantic retrieval, concordance work and RAG systems.

---

**Lux Kybernetica — 2026**

> **La source vient d’abord. Tout le reste doit pouvoir y revenir.**
