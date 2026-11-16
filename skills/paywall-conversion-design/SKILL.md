---
name: paywall-conversion-design
description: Concevoir, auditer ou réécrire le paywall d'une app ou d'un SaaS — écran d'abonnement, essai gratuit, prix et packaging, moment d'apparition, flux d'annulation — à partir de l'étude de ~3 000 paywalls (Mobbin) et de l'expérience de Jonathan Parra, qui en a conçu plus de 4 700. À utiliser dès qu'on parle de « paywall », de « conversion en abonnement », de « taux d'essai », d'« essai gratuit qui ne convertit pas », de « mur payant », de « prix et packaging », de « trial », de « monétisation d'app », de « rétention et LTV », ou qu'on colle une capture d'écran d'abonnement à améliorer.
---

# Concevoir un paywall qui convertit — et qui garde

La thèse à poser avant tout le reste : **la décision de payer ne se prend pas sur le paywall.** L'utilisateur a souvent décidé avant de le voir, ou décidera après. Le paywall n'est donc pas un écran, c'est **un flux** : tout ce qui, dans l'app, amène à ce moment et le rend naturel.

Corollaire pratique : un paywall magnifique peut perdre contre un paywall laid, et il n'existe **aucun meilleur paywall universel**. Il existe des expériences. Le travail n'est donc pas de trouver le design canonique, mais de choisir le bon moment, de réduire le risque perçu, d'encadrer la valeur, puis de tester des design radicalement différents.

## Le cadre : quatre placements, un seul but

Le paywall peut apparaître à quatre endroits. Choisir le placement est la première décision, avant le design.

| Placement | Quand | Ce qu'il fait bien | Risque |
|---|---|---|---|
| **Fin d'onboarding** | après le quiz, quand le plan est prêt | capitalise sur la personnalisation, se sent comme l'étape suivante | demande de l'argent avant tout usage réel |
| **Déblocage d'une fonctionnalité** | au moment où l'utilisateur veut faire la chose précise | la valeur est déjà désirée, le prix a un référentiel | peut ressembler à un chantage si la fonction est essentielle |
| **Réglages / dans l'app** | à froid, par choix | zéro interruption, capte les motivés | peu de volume |
| **Win-back, avant de partir** | à l'annulation ou au retour | sauve les indécis, propose une alternative | mal fait, il retient de force et abîme la marque |

Un même produit peut avoir les quatre. Mais le premier paywall à construire est celui du parcours principal (fin d'onboarding ou déblocage) : on stabilise ses chiffres avant d'optimiser les autres placements.

## Procédure

### 1. Cadrer : objectif, placement, public, prix

Écrire en tête de travail : quel objectif (démarrages d'essai, conversions directes, LTV, rétention), quel placement, quel utilisateur (déjà convaincu ou froid), quel prix et quelle périodicité existent aujourd'hui. Sans l'objectif, tous les arbitrages suivants sont indécidables — notamment celui de la friction, qui échange du volume contre de la qualité.

### 2. Vendre le résultat avant de demander l'argent

Le paywall ne commence pas au paywall. Ce qui le précède doit avoir vendu **un futur**, pas des fonctionnalités. La référence : Opal fait passer l'utilisateur par un écran qui lui montre combien d'années de sa vie il peut récupérer, puis arrive au paywall — les inscriptions à l'essai passent de 7 % à 17 %.

Ce qui doit être vrai à l'entrée du paywall : l'utilisateur a vu son plan ou son résultat personnalisé, et il sait ce qui va changer pour lui. Si ce n'est pas le cas, corriger l'amont avant de toucher au paywall.

### 3. Choisir la forme du flux

Par ordre d'efficacité observée, et à tester sur son propre trafic :

1. **Paywall multi-pages / multi-écrans.** Fait dérouler l'information progressivement, laisse le temps de traiter la décision. Considéré par le praticien interrogé comme presque toujours supérieur au mono-page — c'est son observation de terrain, à vérifier chez soi.
2. **Pay ramp plutôt que paywall.** Supprimer le mur et ne montrer qu'une action : « récupérer votre semaine offerte » (l'approche de Slopes, inspirée d'Apple) — +25 % de démarrages d'essai sur ce seul changement.
3. **Paywall tableau.** Montre ligne par ligne ce qu'on rate sans s'abonner. Très performant, rare parce que pénible à construire dans les outils d'expérimentation.
4. **Paywall vidéo.** Communique la valeur plus vite qu'une capture ou une liste de bullets.
5. **Paywall long format** (beaucoup de texte, très dense). Le cas le plus contre-intuitif : un paywall objectivement laid et agressif a surperformé tous les redesigns sur une app grand public. Ne pas l'écarter par principe.

Le principe de choix : **est-ce que le paywall se sent comme la suite naturelle du parcours, ou comme un mur ?** Si l'utilisateur vient de finir son onboarding et de voir son plan, un écran qui conclut ce parcours se sent juste.

### 4. Réduire le risque perçu

Les hésitations réelles ne portent pas sur le prix mais sur la peur : « vais-je oublier d'annuler ? », « est-ce le bon choix ? ». Les leviers qui marchent :

- **Une timeline d'essai explicite** : aujourd'hui essai gratuit → date de rappel → date de fin → prix ensuite. Blinkist l'a fait et a obtenu plus d'inscriptions, moins de plaintes, et plus d'opt-ins aux notifications (elles rappellent avant la fin, ce qui est cohérent).
- **« Sans engagement, annulable à tout moment »** en sous-titre du bouton : gain incrémental, peu coûteux.
- **L'offre présentée plus clairement, sans changer l'offre** : essai mis en avant, badge de réduction, libellé compréhensible — chez Tipstop, les conversions directes ont triplé à offre identique.
- **Un CTA qui nomme l'action** de l'utilisateur plutôt que « Continuer », et un chevron à droite du bouton : le praticien l'observe sur la majorité des paywalls gagnants, sans avoir encore isolé le chevron dans un test propre.
- **Une feuille d'intention de sortie** à l'annulation : « pas prêt pour un an ? le mensuel existe » — proposition d'alternative, pas rétention forcée.

### 5. Décider de la friction — explicitement

La friction n'est pas l'ennemie de la conversion : elle filtre. Sur Outsider, exiger la carte bancaire a fait **chuter les inscriptions de plus de moitié** mais **multiplié par cinq le taux de conversion**, avec plus du double de clients payants au bout.

Donc la question n'est pas « faut-il de la friction ? » mais **qu'est-ce qu'on optimise** :

- **Volume d'essais, croissance rapide, base large** → pas de carte, essai en un tap.
- **Qualité des essais, revenu, LTV** → carte requise, et assumer la chute des inscriptions.
- **Solution intermédiaire** : essai gratuit réservé à la formule annuelle (l'approche de Moonly), ce qui filtre sans bloquer l'entrée.

Écrire le choix et sa raison dans le rapport : c'est l'arbitrage que la plupart des équipes font par défaut sans le décider.

### 6. Prix et packaging

- **Annuel par défaut** : c'est ce qui donne le meilleur LTV dans la plupart des cas — mais pas dans tous, donc le vérifier plutôt que l'appliquer.
- **Deux options visibles au maximum.** Une troisième option charge cognitivement et dilue la décision.
- **Le reste derrière un bouton** « voir toutes les offres » qui ouvre une feuille listant hebdo, mensuel, annuel.
- **Un essai plus long peut battre une offre moins chère.** Headspace a testé 7, 14 et 30 jours sur l'annuel : c'est le 14 jours sur l'annuel qui a gagné, alors que l'annuel coûte plus cher — parce que l'essai long rend la décision moins risquée.
- **Un prix ancré** : montant hebdomadaire plutôt que mensuel (Tide), ou comparaison avec une dépense familière — un café, une séance de thérapie.

### 7. Rédiger la copie

Titre = le futur de l'utilisateur. Sous-titre = la réduction de risque. Bullets = les bénéfices, pas les fonctionnalités. CTA = le verbe de l'action. Ordre de lecture : valeur, preuve, prix, risque, bouton.

Banque de formulations prêtes à adapter, avec les variantes par type d'app : `references/copy-paywall.md`.

### 8. Mesurer — et pas seulement la conversion

La conversion n'est pas le but, c'est l'entrée. Les métriques qui comptent sont **la rétention et la LTV** : un paywall qui gonfle les inscriptions d'essai et fait churner au troisième jour détruit de la valeur.

Nommer l'événement de chaque étape : vue du paywall, clic sur le CTA, début d'essai, conversion en payant, annulation (avec la raison), renouvellement. Et **le test avant/après** : ce sont les tests de design radicalement différents — vidéo contre liste, tableau contre timeline, long format contre mono-page — qui déplacent le plus l'aiguille, bien plus que les micro-ajustements de copy.

## Le format de livraison

**Calibrer la longueur sur la demande.** C'est la règle qui se rate le plus souvent, donc elle a des budgets :

- « Tu changerais quoi en premier ? », « un avis ? », une question fermée → **15 à 25 lignes** : verdict, 3 actions, rien d'autre. Pas de tableau, pas de section « à mesurer », pas de flux écran par écran.
- « Réécris la copie » → **la copie + un tableau court** de ce qui change et pourquoi. Pas l'audit complet.
- « Refais mon paywall », « audit complet » → le format ci-dessous, en entier.

Quand la demande est courte, la copie réécrite et les trois premières actions suffisent : le reste est du volume que personne n'a demandé.

**Ne jamais inventer un chiffre dans la copie livrée.** Note d'avis, nombre d'utilisateurs, date de renouvellement, montant économisé : chacun s'écrit en gabarit (`4,8 ★ · <nombre réel> avis`, `renouvellement le <date>`), jamais rempli au hasard. Un faux chiffre recopié tel quel dans un paywall en production est une tromperie, et c'est la première chose qu'un utilisateur méfiant vérifie.

```
# Paywall — <app ou écran>
Objectif : ... | Placement : ... | Public : ... | Prix actuel : ...
Hypothèses : ...
## Verdict en une phrase
## À changer en premier (3 max, avec le chiffre ou le mécanisme en appui)
## Le flux cible, écran par écran (avec le rôle de chaque écran)
## La copie exacte — titre, sous-titre, bullets, CTA, mention de risque
## Prix et packaging proposés (et ce que je garde)
## Friction : carte requise ou non, et pourquoi
## Ce que je ne changerais pas (et pourquoi)
## À mesurer avant / après — métrique, événement, durée du test
```

La section « ce que je ne changerais pas » est obligatoire : elle évite de casser un paywall qui convertit déjà, et c'est fréquent — le paywall laid qui gagne est un cas réel, pas une anecdote.

## Repères chiffrés

À traiter comme des cas isolés rapportés par l'étude, jamais comme des garanties — chaque chiffre dépend du produit, du prix et de l'audience.

| Cas | Changement | Résultat |
|---|---|---|
| Opal | vendre les années de vie récupérées avant le paywall | inscriptions à l'essai 7 % → 17 % |
| Tipstop | offre inchangée, présentation clarifiée (essai, badge, libellé) | conversions directes ×3 |
| Slopes | suppression du paywall au profit d'un pay ramp « récupérer votre semaine offerte » | démarrages d'essai +25 % |
| Outsider | carte bancaire exigée pour l'essai | inscriptions −50 %+, conversion ×5, clients payants ×2+ |
| Blinkist | timeline d'essai étape par étape | plus d'inscriptions, moins de plaintes, plus d'opt-ins push |
| Headspace | essai 7 / 14 / 30 jours sur l'annuel | 14 jours gagnant |
| ClassPass | (contre-exemple) | < 5 écrans pour s'abonner, 17 pour annuler |

## Ce qu'il ne faut pas copier

- **La roue de la fortune prédéterminée.** Elle fonctionne, y compris chez les praticiens qui la désapprouvent — mais elle sature : dès que tout le monde l'utilise, les utilisateurs cessent d'y croire. Rentable à court terme sur un prix hebdomadaire, contre-productif sur une marque qu'on veut garder.
- **L'urgence inventée.** Les utilisateurs ont appris qu'une offre arrive après avoir fermé le paywall : ils ferment désormais par réflexe. Une offre unique qui disparaît (one-time offer) reste efficace, mais elle se paie en confiance si elle est fausse.
- **Les remises de dernière minute** sur le bouton d'annulation : à réserver aux vraies périodes promo (Black Friday, Cyber Monday). Une alternative préférable et sûre : **un essai plus long**.
- **Le toggle « essai gratuit » ambigu.** Début 2026, Apple a commencé à rejeter des paywalls dont ce mécanisme était jugé trompeur. La conformité n'est pas un détail de fin de projet : un paywall rejeté, c'est zéro revenu.
- **L'annulation rendue difficile.** Le déséquilibre entre l'inscription (5 écrans) et l'annulation (17 écrans) se retourne en avis négatifs, en remboursements et en rétention de façade.

## Les erreurs qui coûtent

- **Traiter le paywall comme un écran** et ne travailler que dessus, alors que la décision se joue avant.
- **Optimiser la conversion d'essai** sans regarder la rétention : on achète des abonnés qui partent.
- **Empiler les techniques de persuasion** (preuve sociale + ancrage + urgence + remise + roue) : chacune consomme du crédit de confiance.
- **Changer dix choses à la fois** : plus aucun apprentissage possible. Un test, une hypothèse.
- **Copier le paywall d'une app à la mode** sans regarder son prix, son audience et son moment de valeur.
- **Croire que la finition est cosmétique.** À produit équivalent, c'est elle qui départage : animation, branding, univers. Le niveau a monté parce que tout le monde peut publier une app.
