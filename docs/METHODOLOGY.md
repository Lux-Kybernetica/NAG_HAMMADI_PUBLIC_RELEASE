# Méthodologie

## 1. Objet

Le corpus français est conçu comme une couche de traduction de recherche alignée sur des textes anglais redistribuables et documentés.

Il vise quatre propriétés :

1. **fidélité documentaire** ;
2. **traçabilité** ;
3. **alignement stable** ;
4. **exploitabilité informatique**.

## 2. Nature de la traduction

La majorité de la couche française repose sur une traduction anglaise intermédiaire.

Elle ne doit donc jamais être présentée comme :

- une traduction directe du copte ;
- une nouvelle édition critique du manuscrit ;
- une adjudication philologique définitive.

Le statut recommandé est :

> **Traduction française de recherche via un intermédiaire anglais documenté.**

## 3. Segmentation

Chaque œuvre possède des segments stables.

Les fichiers français utilisent notamment :

```text
SOURCE-ID
TARGET-ID
KIND
```

Le texte anglais correspondant est conservé dans un bloc documentaire HTML, suivi de la traduction française.

Cette structure permet une comparaison automatisée et un retour précis à la source utilisée.

## 4. Signaux éditoriaux

Les traductions préservent autant que possible :

- les restitutions `[ ]` ;
- les corrections `< >` ;
- les parenthèses éditoriales `( )` ;
- les lacunes et ellipses ;
- les notes ;
- les divisions et intertitres ;
- les marqueurs et liens de pages.

Les changements de nombre de délimiteurs ne sont pas acceptés silencieusement. Lorsqu’une construction française impose une géométrie différente sans changer le statut épistémique des lexèmes, une exception documentée peut être enregistrée.

## 5. Validation structurelle

Le rail complet comporte :

- **45 œuvres** ;
- **6 670 segments alignés** ;
- **45 / 45 clôtures structurelles PASS** ;
- **0 erreur structurelle** ;
- **0 warning structurel non adjudiqué** ;
- **19 exceptions documentées** au dernier rapport de clôture utilisé pour cette publication.

Les validations contrôlent notamment :

- nombre et ordre des segments ;
- identité du SHA source déclaré ;
- présence des traductions ;
- géométrie des crochets ;
- parenthèses ;
- chevrons ;
- ellipses ;
- marqueurs de pages ;
- plusieurs sentinelles lexicales et migrations de portée.

## 6. Ce que la validation ne prouve pas

Un validateur structurel ne peut pas garantir qu’une phrase française est sémantiquement juste simplement parce qu’elle contient le bon nombre de crochets.

La revue sémantique reste donc une couche distincte.

Le projet distingue au minimum :

```text
TRANSLATED
STRUCTURE_VALIDATED
SEMANTIC_REVIEWED
PHILOLOGICALLY_ADJUDICATED
```

Ces statuts ne doivent pas être confondus.

## 7. Audit contradictoire

Une revue adversariale du rail complet a été utilisée pour chercher des défauts plutôt que pour confirmer passivement le corpus.

Elle a confirmé la clôture structurelle tout en mettant en évidence des sujets de révision sémantique et de gouvernance terminologique.

Cette distinction est conservée dans la publication publique.

## 8. Terminologie

Le corpus utilise un glossaire transversal, mais certaines traductions dépendent du contexte.

Exemple actif : `Fullness`, rendu selon les passages par **plérôme** ou **plénitude**, fait encore l’objet d’une adjudication de gouvernance terminologique.

Une normalisation globale aveugle est interdite lorsque le contexte peut justifier plusieurs rendus.

## 9. Philosophie du corpus

Le but n’est pas d’effacer les difficultés des manuscrits.

Une lacune doit rester une lacune.
Un témoin fragmentaire doit rester fragmentaire.
Une reconstruction doit rester identifiable comme reconstruction.
Une variante ne doit pas être silencieusement harmonisée avec une autre.

> **La source vient d’abord.**
