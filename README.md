# Copilote de l'agent accompagnateur IA · réseau CCI

Un projet Claude pour les conseillers CCI qui accompagnent une TPE ou une PME dans sa démarche vers l'IA : des instructions permanentes, une boussole et 11 skills, un par étape de la méthode, plus 3 notebooks NotebookLM pour se documenter.

Conçu par **Sébastien GRILLOT**, formateur IA, pour la formation CCI Académie « Accompagner une entreprise dans sa démarche vers l'IA » (niveau 2).

## Contenu

| Dossier / fichier | Rôle |
|---|---|
| [`INSTRUCTIONS-PROJET.md`](INSTRUCTIONS-PROJET.md) | Le socle : à coller dans les **instructions du projet** Claude (ce n'est pas un skill) |
| [`skills/`](skills) | La boussole + 11 skills, un dossier par skill avec son `SKILL.md` |
| [`notebooks/`](notebooks) | La méthode pour monter un notebook NotebookLM + les sources des 3 notebooks |

## Les skills

| Skill | Rôle |
|---|---|
| [`boussole-accompagnement-ia`](skills/boussole-accompagnement-ia/SKILL.md) | Point d’entrée : accueille l’agent et l’oriente vers le bon skill |
| [`decouverte-entreprise-ia`](skills/decouverte-entreprise-ia/SKILL.md) | 1 · Découvrir l’entreprise (4 blocs, questions par secteur) |
| [`maturite-numerique-ia`](skills/maturite-numerique-ia/SKILL.md) | 2 · Noter la maturité numérique et IA (0 à 4, sur preuve) |
| [`mise-a-niveau-ia`](skills/mise-a-niveau-ia/SKILL.md) | 3 · Calibrer et fournir la mise à niveau IA |
| [`ideation-cas-usage`](skills/ideation-cas-usage/SKILL.md) | 4 · Faire émerger les cas d’usage (fiches idées) |
| [`approfondissement-idees`](skills/approfondissement-idees/SKILL.md) | 5 · Trier, creuser, éprouver les idées |
| [`portefeuille-priorisation`](skills/portefeuille-priorisation/SKILL.md) | 6 · Peser et prioriser le portefeuille |
| [`formalisation-cahier-besoins`](skills/formalisation-cahier-besoins/SKILL.md) | 7 · Formaliser le besoin (cahier des besoins) |
| [`comprendre-ia`](skills/comprendre-ia/SKILL.md) | Transverse · expliquer les familles d’IA |
| [`trouver-qualifier-donnees`](skills/trouver-qualifier-donnees/SKILL.md) | Transverse · trouver et qualifier les données |
| [`posture-accompagnateur`](skills/posture-accompagnateur/SKILL.md) | Socle · la posture de l’accompagnateur |
| [`atelier-risques-charte-ia`](skills/atelier-risques-charte-ia/SKILL.md) | Gouvernance · atelier risques et charte IA |

Les 7 skills d'étape suivent la méthode de la formation : découverte → maturité → mise à niveau → idéation → approfondissement → portefeuille → formalisation.

## Installation

**Dans Claude (claude.ai ou application) :**
1. Créez un projet et collez le contenu de `INSTRUCTIONS-PROJET.md` dans ses instructions.
2. Ajoutez les skills : téléchargez ce dépôt (Code › Download ZIP), puis importez chaque dossier de `skills/` (zippé) dans Paramètres › Capacités › Skills.

**Dans Claude Code :** copiez les dossiers de `skills/` dans `~/.claude/skills/`.

**Avec un autre assistant (Copilot, ChatGPT, Gemini…) :** collez `INSTRUCTIONS-PROJET.md` dans les instructions personnalisées, puis le `SKILL.md` de l'étape dont vous avez besoin.

## Les notebooks NotebookLM

| Notebook | Pour quoi faire |
|---|---|
| [Comprendre l'IA & savoir quoi suivre](notebooks/01-comprendre-ia-et-savoir-quoi-suivre.md) | Culture IA de fond + repères pour suivre l'actu |
| [Auditer avant de rédiger un cahier des charges](notebooks/02-auditer-avant-de-rediger-un-cahier-des-charges.md) | Comprendre l'existant avant d'écrire |
| [Le champ des possibles & rédiger un cahier des charges IA](notebooks/03-champ-des-possibles-et-cahier-des-charges-ia.md) | Ce que l'IA permet, et comment le traduire en cahier des charges |

Chaque fiche liste les sources à charger ; la [méthode](notebooks/00-methode-notebooklm.md) explique comment monter le notebook.

## À savoir

- Les exemples et les banques de questions sont ancrés sur le territoire du Sud (Provence, Bouches-du-Rhône) : adaptez-les à votre territoire.
- Les liens des sources ont été vérifiés en juillet 2026 ; revérifiez-les avant usage.
- Version du 5 octobre 2026.

Contact : Sébastien GRILLOT · sebastien@koeki.fr
