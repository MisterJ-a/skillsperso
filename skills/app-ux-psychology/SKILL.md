---
name: app-ux-psychology
description: Auditer, corriger ou concevoir l'interface d'une app (web ou mobile) avec cinq leviers de psychologie UX — gradient d'objectif, règle pic-fin, illusion de l'effort, effet Von Restorff, surcharge de choix. À utiliser dès qu'on demande pourquoi une app « ne feel pas », pourquoi les utilisateurs abandonnent un onboarding, un paiement ou une inscription, comment rendre un écran plus agréable ou plus convaincant, ou qu'on colle une maquette, un screenshot ou du code d'écran à améliorer.
---

# Améliorer une app avec la psychologie UX

Cinq leviers tirés de la psychologie cognitive, applicables à n'importe quel écran : ce qui donne à une app cette impression d'être « bonne » sans qu'on sache dire pourquoi — et ce qui la rend pénible sans qu'on sache dire pourquoi non plus.

Le principe de travail : **ne jamais habiller un écran, toujours expliquer le mécanisme**. Un correctif sans le levier qui le justifie est un avis de goût ; le même correctif nommé est une décision qu'on peut défendre, mesurer et généraliser.

## Les cinq leviers

| Levier | Symptôme quand il manque | Ce qu'on ajoute |
|---|---|---|
| **Gradient d'objectif** | Tâches présentées à plat, abandon en cours de parcours | Progression visible (« 3 sur 7 », barre, temps restant) |
| **Règle pic-fin** | Parcours long dont on ne retient que la friction | Un pic marquant + une fin réussie et chaleureuse |
| **Illusion de l'effort** | Actions sensibles expédiées en un clin d'œil, rassurantes à tort | Un temps visible et honnête sur ce qui compte |
| **Effet Von Restorff** | Tout se ressemble, l'œil ne sait pas où aller | Un seul élément qui tranche par écran |
| **Surcharge de choix** | Menus pleins, l'utilisateur hésite et repart | Filtres, catégories, suppression d'options |

Détail de chaque levier — mécanisme, signaux à repérer, correctifs, micro-textes prêts à l'emploi, métrique à suivre : `references/principes.md`. Le lire en entier avant de diagnostiquer, c'est là que se trouvent les formulations exactes.

## Procédure

### 1. Cadrer l'écran et l'objectif

Identifier : quel écran ou quel parcours, quel utilisateur, quel objectif business (activation, conversion, rétention), quel support (mobile, web, app native), et sous quelle forme on l'a (screenshot, maquette Figma décrite, code, URL). Si le contexte manque, avancer avec des hypothèses explicites en tête de rapport plutôt que d'attendre : « je suppose un onboarding mobile pour une app grand public ».

### 2. Inventorier ce qui est à l'écran

Lister, dans l'ordre de lecture de l'utilisateur, chaque zone et chaque élément : titres, champs, boutons, navigation, textes secondaires, états vides, messages d'erreur, écrans de chargement et de succès. Un parcours se juge sur l'ensemble, pas sur l'écran principal : la règle pic-fin et l'illusion de l'effort se jouent dans les transitions.

### 3. Passer les cinq leviers, un par un

Pour chacun, dans cet ordre : chercher le **symptôme** dans l'inventaire, dire s'il s'applique ou non — un levier écarté avec sa raison vaut mieux qu'un levier forcé pour remplir le rapport — puis proposer un **correctif concret** : le composant, le texte exact à afficher, l'état à créer. Jamais de conseil qui ne se traduit pas en quelque chose à dessiner ou à coder.

### 4. Prioriser

Classer les correctifs par impact attendu sur l'objectif de l'étape 1, puis par effort. Trois correctifs à fort impact battent dix remarques ; le rapport le dit en tête.

### 5. Livrer

**Calibrer la longueur sur la demande.** « Audit rapide », « une idée ? », une question sur un seul écran : verdict en une phrase + les 3 actions, dix à quinze lignes, pas de rapport complet. Le format ci-dessous est le format long, pour une demande d'audit complet ou un écran à retravailler sérieusement. Un rapport de 800 mots pour une question de deux lignes est un échec, même juste sur le fond.

Format long par défaut, dans la langue de l'utilisateur :

```
# Audit UX — <écran ou parcours>
Objectif : ... | Hypothèses : ...
## Verdict en une phrase
## À faire en premier (3 max, avec le levier en appui)
## Levier par levier
### <Nom du levier> — s'applique / ne s'applique pas
Symptôme observé : ... (citation de l'écran)
Correctif : ... (texte exact, composant exact)
Effet attendu : ... (mécanisme, puis métrique)
## Écrans ou états à créer
## Ce que je ne changerais pas (et pourquoi)
```

La dernière section compte autant que les autres : elle évite que le prochain passage casse ce qui fonctionne, et elle montre que l'audit distingue l'essentiel du cosmétique.

### 6. Appliquer et vérifier

Si on demande de modifier le code ou la maquette, appliquer uniquement les correctifs validés, un levier à la fois, et rendre l'écran modifié visible (aperçu, capture, lien). Puis vérifier ce qui est vérifiable sans utilisateurs : la progression s'affiche-t-elle dès la première étape ? L'écran de succès existe-t-il sur chaque parcours ? Combien d'éléments concurrents par écran ? Le reste (taux de complétion, abandon) demande une mesure réelle : nommer la métrique et l'événement à instrumenter, ne pas prétendre à un résultat.

## Rédiger les micro-textes

Le levier ne produit son effet que si le mot est juste. Règles :

- **Un chiffre plutôt qu'un adjectif.** « 3 sur 7 » et non « presque fini » ; « environ 2 minutes » et non « bientôt ».
- **Ce qui reste à faire, formulé comme un gain**, pas comme une obligation : « 2 étapes et votre compte est prêt ».
- **Le succès nomme ce qui vient d'être accompli**, pas « Succès ! » tout seul : « Votre dossier est envoyé — réponse sous 48 h ».
- **L'erreur dit quoi faire**, jamais seulement ce qui a échoué.
- Pas d'exclamation en série, pas de félicitations vides : le renforcement positif ne fonctionne que s'il est rare et vrai.

## Limites à ne pas franchir

- **Illusion de l'effort : jamais de faux.** On rend visible un travail réel (vérification, contrôle, envoi) ; on n'ajoute pas une attente inventée pour un paiement, une suppression ou un accès, et jamais plus de quelques secondes. Un délai artificiel sur une action critique se paie en confiance, et sur un parcours répété (usage quotidien, power users) il devient une nuisance.
- **Pic-fin : la fin doit être vraie.** Un écran de succès qui célèbre une action non aboutie détruit la confiance au premier échec.
- **Von Restorff : un seul élément qui tranche par écran.** Deux accents de force égale annulent l'effet et créent le bruit qu'on voulait éviter.
- **Surcharge de choix : supprimer avant de masquer.** Un menu caché qui garde trente entrées reste une surcharge, déplacée.
- Accessibilité non négociable : la progression ne repose pas seulement sur la couleur, l'élément mis en avant reste lisible et atteignable au clavier, les animations respectent `prefers-reduced-motion`.
