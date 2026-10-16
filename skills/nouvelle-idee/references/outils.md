# Règles de choix des outils

Principe. On commence toujours par le plus simple. On ne monte d'un cran que si le cran du dessous ne suffit pas.

## Où travailler
- Conversation Claude (app ou web). Réfléchir, cadrer, chercher, rédiger, maquetter, produire un document, un deck ou une petite page HTML. Les tâches longues avec fichiers s'y font aussi (ce qui s'appelait Cowork).
- Claude Code (sur l'ordinateur de l'utilisateur). Dès qu'il faut un vrai projet avec plusieurs fichiers, du code à lancer, des tests, GitHub, un déploiement.
- n8n (en local ou hébergé). Une tâche qui doit tourner seule, de façon répétée ou planifiée, entre plusieurs services (mail, Google, RSS, API). Les appels IA se font dans un nœud du workflow.
- Lovable. Prototype d'interface très rapide quand l'apparence compte plus que la logique.
- Combinaison fréquente. Cadrage en conversation, construction dans Claude Code, automatisation dans n8n.

## Quel modèle
- Sonnet. Par défaut pour presque tout.
- Opus. Architecture d'un projet, bug qui résiste, raisonnement long. À réserver, il coûte plus cher.
- Haiku. Appels répétés et simples dans n8n ou une appli (classer, résumer, extraire). Le moins cher.
Dans une appli, préférer du contenu pré-généré à des appels IA à chaque utilisation.

## Workflow fixe ou agent
- Workflow fixe. Les étapes sont connues à l'avance. C'est le cas le plus fréquent. Plus fiable, moins cher, plus facile à déboguer.
- Agent. L'IA doit choisir elle-même ses étapes et ses outils selon la situation. À n'utiliser que si un workflow fixe ne suffit pas.
- Sous-agents dans Claude Code. Utiles pour une tâche bien délimitée qui reviendra souvent (revue de code, tests, contrôle design, SEO). Un projet de MVP en demande zéro ou un, rarement plus.

## Connecteurs et MCP
- Vérifier d'abord ce qui est déjà connecté (Figma, Canva, Netlify, Google...).
- Figma. Lire une maquette pour la coder, ou pousser un écran dans Figma.
- Netlify. Mettre en ligne un site ou une appli web gratuitement.
- Canva. Visuels, couvertures, posts.
- Si un service manque, chercher s'il existe un connecteur avant de proposer un développement.

## Skills utiles si elles sont installées
- frontend-design, ui-ux-pro-max, mobile-native, apple-design. Interfaces.
- studio-ebook-kdp. Ebooks et produits digitaux (dans ce dépôt).
- humanizer. Relecture des textes publiés.
- mcp-builder. Créer son propre connecteur.
- skill-creator. Transformer une routine qui revient en skill.

## Estimation de temps (ordres de grandeur pour un non-développeur)
- Page ou mini-outil HTML. 1 à 2 heures.
- Workflow n8n simple. 1 à 3 heures.
- Appli web mobile MVP. 2 à 4 sessions de 2 heures.
- Produit digital (ebook court). 2 à 5 sessions.
Donner une fourchette honnête et signaler ce qui peut la faire déraper.

## Vérification et qualité
- Toute interface est testée sur un vrai téléphone avant d'être considérée comme terminée.
- Code. Tests simples sur ce qui compte, revue de code avant mise en ligne.
- Workflow n8n. Exécution de test avec de vraies données, puis surveillance des premières exécutions.
- Texte publié. Passage par humanizer.
