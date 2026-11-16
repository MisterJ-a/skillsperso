---
name: onboarding-flow-design
description: Concevoir, auditer ou raccourcir un onboarding d'app ou de SaaS — inscription, quiz, permissions, paywall, premier écran — à partir de l'étude de 1 460 flux d'onboarding. À utiliser dès qu'on parle d'onboarding, de "taux d'activation", de "les gens s'inscrivent mais n'utilisent pas", d'écran de bienvenue, de quiz d'inscription, d'essai gratuit qui ne convertit pas, de paywall placé pendant l'inscription, ou qu'on demande s'il faut supprimer / raccourcir l'onboarding.
---

# Concevoir un onboarding qui amène à la valeur

L'idée reçue à jeter tout de suite : « un bon onboarding est court ». Sur 1 460 flux étudiés, l'app moyenne a **25 écrans d'onboarding**, et Duolingo en compte une soixantaine avant même l'inscription — sans que ça paraisse long. La longueur n'est pas la métrique. La seule qui compte : **le temps et l'effort avant le premier moment où l'utilisateur ressent la valeur**.

## Le cadre en trois temps

```
Inscription  →  Mise en place du compte  →  Aha moment
```

Le travail commence toujours par la deuxième flèche : **nommer le aha moment**, en une phrase concrète, avant de dessiner quoi que ce soit.

- Airbnb : faire sa première réservation.
- Netflix : trouver et regarder une série.
- Mobbin : trouver un écran ou une animation qui plaît, et l'enregistrer dans sa collection.
- Un outil de facturation : envoyer sa première facture.

Si on n'arrive pas à nommer ce moment en une phrase vérifiable, l'onboarding ne peut pas être bon : il n'a pas de destination. C'est la première question à poser, avant toute critique d'écran.

Une fois le aha moment nommé, tout l'onboarding se conçoit **à rebours** : quelle est la plus petite chose à demander à l'utilisateur pour qu'il l'atteigne ?

## Procédure

### 1. Nommer le aha moment et le mesurer

Écrire : « L'utilisateur a de la valeur quand ______. » Puis l'événement analytique qui le prouve (`first_invoice_sent`, `first_booking_completed`). Sans cet événement, un onboarding s'optimise à l'aveugle : on ne saura jamais si les écrans ajoutés servent ou retardent.

### 2. Compter les écrans et les classer

Inventorier chaque écran du parcours réel, dans l'ordre, et le ranger dans une catégorie :

| Catégorie | Rôle | Question à se poser |
|---|---|---|
| **Pitch** | vendre le résultat | vend-il le résultat ou liste-t-il des fonctionnalités ? |
| **Personnalisation** | poser 2-5 questions utiles | chaque réponse change-t-elle vraiment quelque chose ? |
| **Éducation** | enseigner au moment où ça sert | est-ce au bon moment, ou tout au début ? |
| **Permission** | notifications, localisation, appareil photo | l'écran de contexte précède-t-il le pop-up système ? |
| **Paywall** | demande d'argent | arrive-t-il avant ou après le aha moment ? |
| **Friction technique** | mot de passe, vérification, formulaire | peut-on le supprimer, le décaler ou l'alléger ? |
| **Aha** | le moment de valeur | est-il atteint, et à quel écran ? |

Un parcours sain n'a pas « trop d'écrans » : il a **les bons écrans dans le bon ordre**, et le aha moment assez tôt.

### 3. Passer les sept leviers

Pour chacun : le symptôme est-il là ? Si non, le dire et passer — un levier écarté avec sa raison vaut mieux qu'un levier forcé. Le détail, les exemples chiffrés et les micro-textes sont dans `references/patterns.md` ; lire le fichier du levier avant de proposer un correctif dessus.

1. **Vendre le résultat, pas les fonctionnalités.** Montrer le produit en action (écran de bienvenue qui montre l'app, animation, ou essai avant inscription), ou un simple changement de copy avec preuve sociale.
2. **Faire humain.** Mot du fondateur, signature manuscrite, note personnelle après la création du compte, message au moment du aha moment. Coût quasi nul, effet mémorable.
3. **Personnaliser — et le rendre utile.** Poser des questions dont les réponses changent l'expérience, autoriser plusieurs intentions plutôt qu'une seule, et rendre les questions conversationnelles.
4. **Montrer le résultat personnalisé.** Après le quiz, afficher ce que les réponses ont débloqué : le plan, la date d'objectif, les contenus sélectionnés. L'utilisateur n'a pas encore utilisé le produit qu'il projette déjà son succès.
5. **Rendre le long court.** Animations, états de chargement soignés, valeur réaffirmée, progression : un flux long peut être agréable ; un flux court et terne reste une corvée.
6. **Enseigner au bon moment.** Tooltips qui expliquent l'impact d'une étape, microcopy rassurante sur un concept aride, validation en direct d'un champ, état vide qui montre à quoi ressemble un compte rempli. Pas de visite guidée au début.
7. **Demander au bon moment.** Un écran de contexte avant chaque pop-up système, la notification annoncée dans son bénéfice, le paywall après la valeur démontrée — ou assumé comme test, mais alors mesuré.

### 4. Trancher : faut-il un onboarding du tout ?

Pour certains produits, la meilleure expérience est de laisser entrer vite. Le test : **est-ce que le premier geste dans le produit EST la valeur ?** Une app de chat IA : le premier prompt est la valeur, pas un tutoriel. Un moteur de recherche d'inspiration : le premier écran trouvé est la valeur. Dans ces cas, l'onboarding doit s'effacer, pas se perfectionner — un écran de bienvenue y est un péage.

À l'inverse, un produit dont la valeur demande une configuration (données, compte, import, réglages métier) a besoin d'un parcours, parfois long.

### 5. Livrer

**Calibrer la longueur sur la demande.** « Un avis sur mon onboarding ? » → le diagnostic en une phrase + 3 actions. « Refais mon parcours » → l'audit complet ci-dessous.

Format long :

```
# Onboarding — <produit ou parcours>
Aha moment : ... (événement : ...)
Hypothèses : ...
## Diagnostic en une phrase
## Le parcours aujourd'hui (tableau écran par écran, avec la catégorie)
## À faire en premier (3 max, avec le levier et le chiffre qui l'appuie)
## Levier par levier — s'applique / ne s'applique pas
Symptôme : ... Correctif : ... Effet attendu : ... Métrique : ...
## Le parcours cible (écran par écran)
## Ce que je ne changerais pas (et pourquoi)
## À mesurer avant / après
```

La section « ce que je ne changerais pas » est obligatoire : elle empêche de casser ce qui marche et distingue l'essentiel du cosmétique.

### 6. Vérifier ce qui est vérifiable

Sans utilisateurs, on peut contrôler : le aha moment est-il atteint avant le paywall ? chaque question du quiz change-t-elle un affichage réel ? y a-t-il un écran de contexte avant chaque pop-up système ? le champ mot de passe valide-t-il ses règles en direct ? l'état vide montre-t-il un exemple ? Y a-t-il une visite guidée au début (à supprimer) ?
Le reste — taux d'activation, conversion, rétention — exige une mesure : nommer la métrique et l'événement, ne jamais annoncer un chiffre de gain.

## Repères chiffrés

À utiliser comme ordres de grandeur, jamais comme promesse. Source : étude Mobbin sur 1 460 flux (voir `references/source-video.md`).

| Repère | Valeur |
|---|---|
| Écrans d'onboarding, moyenne | 25 |
| Flux les plus longs | finance, santé/forme, éducation (7 des 10 plus longs sont finance) |
| Apps qui personnalisent pendant l'onboarding | 23 % (apps IA : 7 %) |
| Apps qui posent un paywall pendant l'onboarding | 22 % (sur 900+ apps et sites) |
| Onboarding web vs iOS | web 21 % plus court (permissions et paywalls en moins) |
| Duolingo | ~60 écrans avant l'inscription, et ça ne « paraît » pas long |

S'y ajouter les gains cités par l'étude, à traiter comme des cas isolés, pas des garanties : multi-intentions (Headspace) +10 % de conversion en essai gratuit ; copy du quiz rendue conversationnelle (Dollar Shave Club) +5 % d'abonnements ; tarifs adaptés au quiz (Grammarly) ~+20 % de montées en gamme ; formulaire d'inscription découpé en plusieurs écrans (House) +15 % de conversions ; checklist à la place des pop-ups (Mural) +10 % de rétention relative à une semaine.

## Les erreurs qui coûtent

- **Lister des fonctionnalités** au lieu de montrer le résultat : l'utilisateur n'a pas encore de raison d'y croire.
- **Tout enseigner au début.** L'éducation au mauvais moment est du bruit ; elle devient invisible quand elle arrive à l'endroit où elle sert.
- **Demander une permission sans contexte.** Le pop-up système arrive avant que l'utilisateur ait compris ce qu'il gagne.
- **Poser des questions qui ne changent rien.** Une question sans effet sur l'expérience est une friction pure, et elle apprend à l'utilisateur à répondre au hasard.
- **Un paywall avant le aha moment**, sans avoir rien démontré : le prix est jugé sans référence de valeur.
- **Imiter ce qui marche ailleurs sans regarder sa culture.** Une interface dense est du désordre pour un public, de l'efficacité pour un autre : la densité d'information attendue varie selon les marchés.
- **Croire que faire court est un objectif.** Couper un écran qui portait la personnalisation rend le parcours plus rapide et moins convaincant.
- **Déplacer la friction au lieu de la supprimer.** Découper un formulaire peut aider (House : +15 %), mais si c'est le seul changement, on a juste réparti la même corvée.
