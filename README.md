# skillsperso

Skills d'agent IA créés à partir de vidéos YouTube. Chaque skill est un dossier sous `skills/`, avec un `SKILL.md` (procédure) et un dossier `references/` (le détail, chargé seulement quand il sert).

## Installation

Une seule commande, depuis n'importe où :

```bash
npx skills add MisterJ-a/skillsperso -g -a claude-code
```

Sans `-g`, le skill est installé dans le projet courant (`./.claude/skills/`) au lieu de `~/.claude/skills/`. Remplacer `claude-code` par `cursor`, `codex`, `opencode`, etc. selon l'outil.

Installer un seul skill :

```bash
npx skills add MisterJ-a/skillsperso --skill onboarding-flow-design -g -a claude-code
```

Voir ce que contient le dépôt sans rien installer :

```bash
npx skills add MisterJ-a/skillsperso --list
```

Mettre à jour plus tard, une fois les skills modifiés dans le dépôt :

```bash
npx skills update
```

## Sans `npx`

```bash
git clone https://github.com/MisterJ-a/skillsperso.git /tmp/skillsperso
cp -r /tmp/skillsperso/skills/onboarding-flow-design ~/.claude/skills/
```

Il faut que `~/.claude/skills/onboarding-flow-design/SKILL.md` existe à la fin.

## Les skills

### `app-ux-psychology`

Cinq leviers de psychologie UX pour auditer ou concevoir un écran : gradient d'objectif, règle pic-fin, illusion de l'effort, effet Von Restorff, surcharge de choix. Procédure d'audit en 6 étapes, format de rapport, garde-fous (jamais de faux délai, un seul accent par écran, accessibilité).

Source : *The psychology trick that makes any app feel 10x better* — Wyatt Feaster.

### `onboarding-flow-design`

Concevoir, auditer ou raccourcir un onboarding : le cadre inscription → mise en place → aha moment, une grille pour classer chaque écran, les 7 leviers, les repères chiffrés de l'étude Mobbin sur 1 460 flux, et les erreurs qui coûtent.

Source : *I Studied 1,460 Onboarding Flows. Here's What I Found.* — Mobbin.

## Ajouter un skill

Créer `skills/<nom-en-kebab-case>/SKILL.md` avec un frontmatter `name` et `description`, et mettre le détail long dans `references/`. Le `name` du frontmatter doit être identique au nom du dossier, sinon `npx skills add --skill <nom>` échoue. Committer, puis `npx skills update` côté utilisateur.

## Notes

- Les skills sont en français ; les sources vidéo sont en anglais et horodatées dans chaque `references/source-video.md`.
- Chaque skill distingue explicitement ce qui vient de la vidéo et ce qui a été ajouté (procédure, garde-fous, métriques).
