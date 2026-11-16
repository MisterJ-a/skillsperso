# Les cinq leviers, en détail

## Sommaire
1. Gradient d'objectif (Goal Gradient Effect)
2. Règle pic-fin (Peak-End Rule)
3. Illusion de l'effort (Labor Illusion)
4. Effet Von Restorff (Von Restorff Effect)
5. Surcharge de choix (Choice Overload)
6. Table de diagnostic rapide

---

## 1. Gradient d'objectif (Goal Gradient Effect)

**Mécanisme.** Le cerveau aime fermer les boucles. Plus on approche d'un objectif, plus la motivation augmente — brutalement. L'image de la vidéo : le coureur épuisé qui retrouve un regain d'énergie à la vue de la ligne d'arrivée.

**Ce que ça donne dans une app.** Les barres de progression, les séries (streaks), la complétion d'onboarding. Les onboardings qui affichent une progression continue ont de meilleurs taux de complétion que ceux qui n'en affichent pas.

**Symptômes à repérer.**
- Une liste de tâches à faire sans indication d'avancement.
- Un onboarding en plusieurs étapes sans compteur ni barre.
- Un formulaire long sans découpage ni repère de position.
- Une progression qui commence à 0 % et reste décourageante (le pire : 0 % sur 10 étapes).
- Une série (streak) qui casse sans recours, ce qui supprime la motivation au lieu de la relancer.

**Correctifs.**
- Afficher la position : « Étape 2 sur 5 », « 3 sur 7 tâches terminées ».
- Démarrer la progression non à zéro quand l'utilisateur a déjà fait quelque chose avant le parcours (compte créé, e-mail vérifié) : la barre reflète le chemin réel, pas l'écran courant.
- Montrer le temps restant quand les étapes sont d'inégale longueur : « environ 2 minutes ».
- Sur une série, offrir un rattrapage plutôt qu'une remise à zéro : un streak perdu définitivement est un streak abandonné.
- Sur un tableau de bord, exprimer l'objectif comme une distance parcourue : « 12 sur 20 cette semaine ».

**Micro-textes.**
- « 3 sur 7 — plus que 4 »
- « Encore 2 étapes, environ 1 minute »
- « Votre profil est complet à 80 % — ajoutez une photo pour le terminer »

**Métrique.** Taux de complétion du parcours, abandon par étape, temps par étape. L'événement à instrumenter : une vue par étape avec son numéro.

**Piège.** Une barre de progression qui n'avance pas (ou recule) après une action produit exactement l'effet inverse : elle signale que l'effort ne paie pas.

---

## 2. Règle pic-fin (Peak-End Rule)

**Mécanisme.** Le cerveau ne garde pas la moyenne d'une expérience : il en retient le moment le plus intense (le pic, bon ou mauvais) et la fin. Le milieu — tout ce qui était « correct » — s'efface.

**Ce que ça donne dans une app.** Airbnb et Duolingo investissent massivement dans les écrans de succès et le renforcement positif : c'est la fin qu'on retiendra. À l'inverse, un parcours long avec un pic de friction (formulaire qui plante, vérification incompréhensible) laisse le souvenir de la friction, même si le reste était fluide.

**Symptômes à repérer.**
- Parcours qui se termine sans confirmation : l'utilisateur reste dans le doute sur ce qui vient de se passer.
- Fin expédiée en une notification technique (« Enregistré. ») après un effort important.
- Pic de friction non traité : l'étape la plus lourde (paiement, pièce d'identité, import de données) est aussi la moins accompagnée.
- Écran de succès générique, identique pour toutes les actions, donc mémorable pour aucune.
- Erreur en fin de parcours : elle devient le souvenir dominant de tout le parcours.

**Correctifs.**
- Créer un vrai écran de fin pour chaque parcours important : ce qui vient d'être accompli, ce qui se passe maintenant, quand arrivera la suite.
- Placer le pic positif au bon endroit : animer ou célébrer l'accomplissement réel, pas l'ouverture de l'app.
- Traiter le pic de friction comme une priorité : expliquer pourquoi l'étape existe, combien de temps elle prend, ce qu'il faut préparer.
- Sur un parcours à étapes, terminer chaque étape sur une petite confirmation avant d'enchaîner.
- Éviter de finir sur une demande (noter l'app, activer les notifications) : la demande se place après la célébration, ou plus tard.

**Micro-textes.**
- « C'est fait. Votre annonce est en ligne et visible par les personnes de votre région. »
- « Paiement confirmé — votre commande part demain, vous recevrez le suivi par e-mail. »
- « Votre dossier est complet. Nous revenons vers vous sous 48 h ; vous pouvez fermer cette page. »

**Métrique.** Satisfaction en fin de parcours (CSAT ou question unique), taux de retour après le parcours, notes et avis. L'événement : la vue de l'écran de succès.

**Piège.** Si la fin ment (succès affiché alors que l'action a échoué), le pic devient négatif et définitif : c'est le type d'incident que les utilisateurs racontent.

---

## 3. Illusion de l'effort (Labor Illusion)

**Mécanisme.** Nous valorisons davantage ce qui a demandé du temps. L'effort perçu crée de la valeur perçue, et l'instantané peut sembler suspect : pour une action sensible, la rapidité enlève le sentiment de sécurité.

**Ce que ça donne dans une app.** Des apps ajoutent volontairement du temps sur des tâches pourtant instantanées — vérification d'un permis de conduire, contrôle d'antécédents — parce que ces tâches sont sensibles : l'utilisateur veut sentir qu'il se passe quelque chose, que quelqu'un a regardé. « Plus rapide » n'est pas toujours mieux.

**Symptômes à repérer.**
- Action sensible terminée instantanément, sans aucune trace du contrôle (le doute s'installe : « ont-ils vraiment vérifié ? »).
- Barre de chargement qui saute de 0 à 100 % ou qui n'explique rien.
- Long parcours sans indication de ce qui se passe en coulisses.
- À l'inverse : attente inventée sur une action triviale ou répétée, qui irrite.

**Correctifs.**
- Sur les actions sensibles (vérification d'identité, contrôle, envoi de dossier, paiement), afficher les étapes réelles du traitement : « Vérification du document… », « Contrôle de conformité… », puis le résultat.
- Traduire l'attente en information : ce qui est en cours, ce que ça garantit, quand ça se termine.
- Utiliser un état de chargement continu et crédible (étapes nommées) plutôt qu'un spinner muet.
- Sur une action répétée et triviale, faire l'inverse : aller vite, sans théâtre.

**Micro-textes.**
- « Nous vérifions votre pièce d'identité — cela prend généralement une minute. »
- « Contrôle en cours : conformité, puis vérification du document. »
- « Vérification terminée. Votre identité est confirmée ; vous n'aurez plus à la refaire. »

**Métrique.** Taux de confiance déclaré, abandon pendant l'attente, taux d'erreur de l'action (« ont-ils bien pris en compte ? »). Événements : début et fin de chaque étape affichée.

**Piège — la limite dure.** Ajouter du temps sur une action qui n'attend rien, sans le dire, est une tromperie : elle se retourne en confiance perdue dès qu'elle est découverte, et elle coûte à chaque usage répété. Règle : rendre visible un travail réel, jamais inventer une attente ; et pas plus de quelques secondes.

---

## 4. Effet Von Restorff (Von Restorff Effect)

**Mécanisme.** Parmi des éléments similaires, on ne retient que celui qui diffère. Le cerveau économise : il repère la rupture, ignore le reste.

**Ce que ça donne dans une app.** Le glacier dont on se souvient n'est pas la vanille ni le chocolat : c'est le parfum bizarre. Les meilleures apps ne déversent pas des listes d'éléments identiques : elles choisissent ce qui mérite l'attention et le distinguent — icône, illustration, taille, couleur, poids typographique.

**Symptômes à repérer.**
- Tous les boutons ont le même poids visuel : l'utilisateur ne sait pas quelle est l'action principale.
- Deux ou trois éléments concurrents mis en avant avec la même force : l'effet s'annule, c'est du bruit.
- Menus et listes uniformes où l'essentiel se noie.
- Écran où « quelque chose cloche » sans qu'on puisse nommer quoi : c'est souvent l'absence de hiérarchie.
- Accent mis sur un élément décoratif plutôt que sur l'action attendue.

**Correctifs.**
- Un seul élément qui tranche par écran : l'action principale, traitée avec la couleur de marque, la taille et l'emplacement dominant.
- Un bouton principal plein, les secondaires en contour ou en texte : la différence doit être visible en plissant les yeux.
- Distinguer les éléments clés d'une liste par une icône ou une illustration, pas seulement par un label.
- Réserver les illustrations et les animations à ce qui doit être mémorisé.
- Vérifier la hiérarchie par un test simple : flouter la capture ; ce qui reste identifiable est la vraie hiérarchie.

**Micro-textes.** Le levier est visuel ; le texte sert à ne pas rivaliser : une seule phrase de valeur par écran, le reste en secondaire discret.

**Métrique.** Taux de clic sur l'action principale vs les secondaires, temps avant le premier clic, erreurs de navigation. Attention : un excès d'accent produit aussi du bruit, la métrique utile est le taux de clic sur l'action attendue.

**Piège.** Plus de deux accents concurrents = zéro accent. Et un accent ne remplace pas une hiérarchie de contenu absente.

---

## 5. Surcharge de choix (Choice Overload)

**Mécanisme.** Devant trop d'options, le cerveau ne peut pas traiter : tension, hésitation, anxiété, puis retrait. Le menu de restaurant à rallonge est le cas d'école ; l'app avec une navigation qui expose tout ce qu'elle contient produit exactement la même réaction.

**Ce que ça donne dans une app.** Les meilleures apps réduisent la fatigue décisionnelle : filtres et recherche pour naviguer dans un grand ensemble, catégories qui regroupent, suppression pure et simple des éléments dont personne n'a besoin.

**Symptômes à repérer.**
- Navigation qui expose toutes les sections au même niveau, sans hiérarchie.
- Écran de réglages interminable : l'utilisateur ne trouve pas, ou renonce.
- Formulaire qui demande tout d'un coup, y compris des champs facultatifs.
- Liste de résultats non filtrable et non triable.
- Écran d'accueil qui propose dix chemins possibles dès l'ouverture.
- Prix ou offres présentés en cinq variantes très proches.

**Correctifs.**
- **Supprimer d'abord** : tout élément dont l'absence ne se remarque pas.
- **Regrouper** ensuite en catégories nommées par la tâche de l'utilisateur, pas par l'organisation interne.
- **Filtrer et rechercher** pour les grands ensembles ; proposer un tri par défaut raisonnable.
- **Progresser** sur les formulaires : le minimum nécessaire d'abord, le reste plus tard ou en option clairement marquée.
- **Recommander** une option par défaut, présentée comme « le choix de la plupart », pour transformer un choix multiple en confirmation.
- Sur les offres, deux ou trois formules maximum, avec une seule mise en avant.

**Micro-textes.**
- « Filtres » plutôt que vingt cases à cocher.
- « Recommandé pour vous » sur l'option par défaut.
- « Vous pourrez compléter ces informations plus tard. »

**Métrique.** Taux de rebond sur les écrans à choix, temps de décision, taux de sortie sans action, taux d'utilisation des filtres.

**Piège.** Masquer sans réduire ne règle rien : un menu déroulant de trente entrées reste trente entrées. Réduire le nombre, puis organiser le reste.

---

## 6. Table de diagnostic rapide

| Ce qu'on observe | Levier probable | Première chose à essayer |
|---|---|---|
| L'utilisateur abandonne au milieu d'un parcours | Gradient d'objectif | Afficher « étape X sur Y » et le temps restant |
| Le parcours se termine dans l'indifférence ou le doute | Pic-fin | Créer un écran de succès qui dit ce qui vient de se passer |
| L'utilisateur doute qu'on ait vraiment vérifié quelque chose | Illusion de l'effort | Nommer les étapes réelles du contrôle |
| On ne sait pas où cliquer | Von Restorff | Un seul bouton plein, les autres en secondaire |
| « Ça fait trop », « je ne sais pas où commencer » | Surcharge de choix | Supprimer, puis regrouper, puis filtrer |
| Une app qui « sent » le travail bien fait sans qu'on puisse dire pourquoi | Les cinq, bien dosés | Ne rien changer : documenter ce qui fonctionne |
