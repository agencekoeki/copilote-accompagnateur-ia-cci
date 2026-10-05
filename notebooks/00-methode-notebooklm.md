# **MÉTHODE — Construire un notebook NotebookLM nickel (les 100 % des étapes)**

> Doc de référence commun. Les trois docs par sujet (Comprendre l'IA / Auditer avant CDC / Champ des possibles) s'appuient dessus. Vérifié en juillet 2026 — NotebookLM bouge vite, revérifie les chiffres avant un engagement.

## **Le principe qui commande tout**

**La qualité des réponses = la qualité et l'organisation de tes sources.** NotebookLM ne répond qu'à partir de ce que tu lui donnes (source-grounded), avec citations. Donc 99 % du travail est en amont : choisir, nettoyer, organiser les bonnes sources. Un notebook mal nourri produit du flou, même avec les meilleurs prompts.

Deuxième principe : **un notebook = un sujet.** On ne mélange pas des thèmes sans rapport. Pour un gros périmètre, on fait plusieurs notebooks (les notebooks ne se parlent pas entre eux — pas de requête d'un notebook à l'autre).

## **Les étapes, dans l'ordre**

**1. Créer et NOMMER le notebook.** Un titre clair et scannable (le sujet, pas « Notebook 1 »). C'est ce que verront ceux à qui tu partages.

**2. Écrire le « README » du notebook (source n°1).** Avant toute autre source, ajoute une courte note-source qui dit : à quoi sert ce notebook, comment il est structuré, et les consignes permanentes. C'est le mode d'emploi, pour toi, pour tes gens, et pour l'IA elle-même.

**3. Rassembler et NETTOYER les sources avant l'upload.** Cinq minutes de nettoyage en amont valent dix fois leur temps en précision : titres clairs, transcripts avec les locuteurs, pas de scans illisibles. **Splitte les gros PDF** (livres, longs rapports) en chapitres/sections logiques avant de les charger — la récupération et les citations sont bien plus nettes.

**4. Choisir le BON nombre de sources.** L'idéal pour la précision : **5 à 10 documents liés**. On peut monter jusqu'à 50 (tier gratuit), mais au-delà de ~15 il faut organiser (voir étape 5), sinon on noie l'IA. Mieux vaut 8 sources excellentes que 40 moyennes.

**5. Organiser les sources en couches.** Range-les mentalement (et par le nommage) en strates :

* **Socle** : concepts fondamentaux, cadre, méthode — ce qu'on lit d'abord.  
* **Substance** : la matière principale, les documents qui comptent le plus.  
* **Support** : annexes, exemples, compléments.  
* **Sorties** : tes propres notes générées, synthèses gardées. Astuce de nommage qui « pirate » le tri : préfixe numérique (`01_`, `02_`, `10_`, `20_`) pour forcer l'ordre d'affichage, + un emoji couleur par couche pour repérer la catégorie d'un coup d'œil. (NotebookLM propose aussi un étiquetage/clustering automatique des sources — utile au-delà de 15 sources.)

**6. Privilégier les sources VIVANTES quand le contenu bouge.** Un Google Doc / Slides / Sheets ajouté comme source est un document *vivant* : tu peux resynchroniser ses mises à jour. Un PDF est *figé*. Pour tout ce qui doit rester à jour (veille, listes), utilise un Google Doc que tu maintiens, pas un PDF.

**7. Configurer le chat (custom instructions).** C'est le levier le plus sous-utilisé. Dans « Configure Chat », ajoute une instruction permanente qui cadre chaque réponse sur l'objectif du notebook et le public (ton, niveau, format). Exemple : « Réponds sans jargon, avec des analogies, pour un non-technique. » Ça change toutes les réponses ET les artefacts.

**8. Interroger intelligemment.** Questions **spécifiques**, pas « parle-moi de ça ». Le bon enchaînement : commencer large (« quels sont les grands thèmes ? ») → creuser (« détaille le point 2, sur quelles preuves ? ») → connecter (« comment ça rejoint la source X ? ») → challenger (« une source contredit-elle ça ? »). Purge l'historique de chat après quelques échanges pour ne pas polluer les suivants (garde d'abord ce qui vaut le coup).

**9. Générer les artefacts utiles (Studio).** Selon le besoin : Résumé audio (podcast, formats deep dive / brief / débat), Résumé vidéo, Carte mentale (interactive), Rapports / briefings, Présentation (export PPTX/PDF), Quiz & Fiches, Infographie, Tableau de données. Les custom instructions s'y appliquent aussi (ex. charte graphique en source

* « suis cette charte » pour l'infographie).

**10. Sauver et exporter.** Épingle les meilleures réponses en Notes ; réarrange ; exporte vers Google Docs/Sheets. Les artefacts se téléchargent (audio en WAV → convertir en MP3, mind map en PNG, slides en PPTX).

**11. Maintenir (5 min/semaine).** Supprimer les doublons, retitrer ce qui est flou, resynchroniser les fichiers Drive périmés. Un notebook figé sur un sujet mouvant se périme — surveille surtout ça.

**12. Partage & confidentialité (à décider AVANT de remplir).** Deux règles dures :

* **« Anyone with a link » n'existe QUE sur compte Gmail perso.** Sur un compte Workspace (`@koeki.fr`), le partage est restreint au domaine — pas de lien public. Donc : notebook destiné à être partagé largement = à créer depuis un **compte perso**.  
* **Partager un notebook expose SES SOURCES.** Ne jamais mettre de données client / transcript / cas réel dans un notebook qu'on rendra public. Pour ça : compte Workspace, partage restreint, ou n'expose que l'artefact exporté (le fichier), pas le notebook.

## **Règles d'or (mémo)**

* Sources propres > prompts malins.  
* 1 notebook = 1 sujet ; 5-10 sources idéales ; organiser dès 15.  
* README en source n°1 + custom instructions dès le départ.  
* Vivant (Google Doc) pour ce qui bouge, figé (PDF) pour ce qui est stable.  
* Public d'un lien = compte perso + contenu non sensible, uniquement.

## **Pièges**

* **Surcharger** (40 sources mélangées) → réponses floues. Cure et sépare en notebooks.  
* **Sources sales** (scans, PDF non titrés) → clustering et citations vagues.  
* **PDF figé pour de la veille** → périmé en silence. Google Doc vivant à la place.  
* **Oublier les custom instructions** → réponses génériques, mauvais ton pour le public.  
* **Créer sur Workspace un notebook qu'on veut public** → pas de lien public possible.  
* **Mettre du sensible dans un notebook public** → fuite des sources.
