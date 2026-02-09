# 	Data Science 07 : Besoins et interactions clients en Data Science

J. Delpech – Cours : Data Science

Cursus M1 Data/IA – 2025/2026

Dernière mise à jour : février 2026

---

**Objectif** : Développer les compétences relationnelles et méthodologiques pour comprendre, cadrer et formaliser les besoins clients dans un contexte Data Science.

---

## 1. Introduction : le Data Scientist, un traducteur

### 1.1 Entre technique et métier

Le Data Scientist occupe une position d'interface dans l'organisation :

![Schéma Data Scientist Interface](./Images/DataScientistInterface.png)

Cette position exige des **compétences hybrides** : excellence technique ET capacité à communiquer avec des non-techniciens.

### 1.2 Importance de la compréhension/traduction

Les conséquences d'une mauvaise compréhension des besoins sont désastreuses :

| Problème | Conséquence |
|----------|-------------|
| Besoin mal compris | Projet qui ne répond pas à l'attente réelle |
| Objectif flou | Impossible de mesurer le succès |
| Contraintes ignorées | Solution inutilisable en production |
| Attentes irréalistes | Déception et perte de confiance |
| Données sous-estimées | Retards, surcoûts, échec du projet |

> Régulièrement des cabinets d’audit ([BCG](https://www.bcg.com/press/24october2024-ai-adoption-in-2024-74-of-companies-struggle-to-achieve-and-scale-value), [Gartner](https://www.gartner.com/en/insights)…) publient des enquêtes selon lesquelles **60-80% des projets data échouent** — et la majorité de ces échecs sont liés à des problèmes de cadrage et de communication, pas à des problèmes techniques.

### 1.3 Solution technique ≠ Valeur business

Une erreur fréquente du Data Scientist débutant : se focaliser sur la solution technique au détriment de la valeur métier.

| Approche technique | Approche orientée valeur |
|-------------------|-------------------------|
| "J'ai construit un modèle avec 95% de précision" | "Le modèle permet de réduire le taux de fraude de 30%" |
| "J'utilise un réseau de neurones profond" | "La solution automatise 70% des cas simples" |
| "L'algorithme est à la pointe de l'état de l'art" | "Le temps de traitement passe de 2 jours à 2 heures" |

**Le client se moque de la technique — il veut résoudre son problème.**

### 1.4 Les parties prenantes d'un projet data

Un projet data implique de nombreux acteurs aux intérêts parfois divergents :

| Partie prenante | Préoccupations principales | Ce qu'il faut comprendre |
|-----------------|---------------------------|-------------------------|
| **Sponsor** (direction) | ROI, budget, délais, risques | Enjeux stratégiques, contraintes budgétaires |
| **Métier** (utilisateurs finaux) | Facilité d'usage, gain de temps, fiabilité | Processus actuels, points de douleur |
| **IT** | Intégration, maintenance, sécurité | Contraintes techniques, architecture existante |
| **Juridique/Conformité** | RGPD, éthique, responsabilité | Contraintes légales, données autorisées |
| **Data** (vous) | Faisabilité, qualité des données, méthodologie | Données disponibles, complexité réelle |

> Attention à ne parler pas qu'aux décideurs : les **utilisateurs finaux** ont souvent une meilleur connaissance du besoin réel.

### 1.5 Cycle de vie d'un projet data



![Schéma cycle de vie projet data](./Images/CycleVieProjetData.png)

**Nous nous concentrons pour cette séance sur les premières phases** : expression du besoin et cadrage — les plus critiques pour le succès du projet.

---

## 2. L'écoute active : fondement de la relation client

### 2.1 Qu'est-ce que l'écoute active ?

L'écoute active est une posture de communication qui va au-delà du simple fait d'entendre. Elle implique :

- **Attention totale** : être pleinement présent, sans préparer sa réponse pendant que l'autre parle
- **Non-jugement** : accueillir ce qui est dit sans évaluer ni critiquer
- **Empathie** : chercher à comprendre le point de vue de l'autre
- **Feedback** : montrer qu'on a compris par la reformulation

### 2.2 Les composantes de l'écoute active

**Verbal** :
- Reformuler : "Si je comprends bien, vous souhaitez..."
- Clarifier : "Pouvez-vous m'en dire plus sur... ?"
- Résumer : "En résumé, les trois points clés sont..."
- Valider : "Est-ce que j'ai bien compris ?"

**Non-verbal** :
- Contact visuel approprié
- Posture ouverte et orientée vers l'interlocuteur
- Hochements de tête, expressions faciales d'intérêt
- Prise de notes (montre l'importance accordée)

**Para-verbal** :
- Ton calme et posé
- Rythme adapté à l'interlocuteur
- Silences permettant la réflexion

### 2.3 La reformulation : l'outil clé

La reformulation est l'outil le plus puissant de l'écoute active. Elle permet de :
- Vérifier qu'on a bien compris
- Montrer au client qu'il est écouté
- Clarifier les ambiguïtés
- Faire progresser l'échange

| Type de reformulation | Exemple |
|-----------------------|---------|
| **Écho** (répéter les mots clés) | Client : "On perd trop de temps sur les réclamations" → Vous : "Trop de temps sur les réclamations..." |
| **Miroir** (reformuler avec ses mots) | "Vous passez beaucoup de temps à traiter les réclamations manuellement" |
| **Synthèse** (résumer plusieurs points) | "Si je résume : le volume de réclamations a augmenté, le traitement est manuel, et cela mobilise deux personnes à temps plein" |
| **Clarification** (vérifier le sens) | "Quand vous dites 'trop de temps', on parle de combien d'heures par semaine ?" |

### 2.4 Adapter son discours

Le Data Scientist doit être un **caméléon linguistique** :

| Interlocuteur | Adapter... | Éviter... |
|---------------|------------|-----------|
| Direction générale | Parler ROI, stratégie, risques | Détails techniques, jargon ML |
| Métier / Utilisateurs | Parler processus, gain de temps, facilité | Algorithmes, architecture |
| IT | Parler intégration, API, performances | Vulgarisation excessive |
| Data Scientists | Parler modèles, métriques, features | ... rien, vous êtes entre pairs ! |

> Règle d'or : soyez attentifs aux signes indirects (non verbaux…) que votre interlocuteurs suit toujours !

---

## 3. Techniques de questionnement

### 3.1 Questions ouvertes vs fermées

| Type | Définition | Quand l'utiliser | Exemples |
|------|------------|------------------|----------|
| **Ouverte** | Appelle une réponse développée | Exploration, compréhension du contexte | "Comment fonctionne votre processus actuel ?" |
| **Fermée** | Appelle oui/non ou réponse courte | Confirmation, précision factuelle | "Combien de réclamations par jour ?" |

**Séquence recommandée** : commencer par des questions ouvertes (exploration), puis resserrer avec des questions fermées (précision).

### 3.2 La méthode Qui / Quoi / Quand (QQOQCCP ou 5W+H)

Une [méthode classique](https://fr.wikipedia.org/wiki/QQOQCCP) (cf. Aristote) pour explorer un sujet de manière exhaustive :

| Question | Application en Data Science |
|----------|----------------------------|
| **Qui** ? | Qui sont les utilisateurs ? Qui décide ? Qui fournit les données ? |
| **Quoi** ? | Quel est le problème ? Quelle décision à prendre ? Quels résultats attendus ? |
| **Où** ? | Où se situe le problème ? Où sont les données ? Où sera déployée la solution ? |
| **Quand** ? | Quand le problème survient-il ? Quels délais ? Quelle fréquence d'utilisation ? |
| **Comment** ? | Comment fonctionne le processus actuel ? Comment sera utilisée la solution ? |
| **Combien** ? | Quel volume de données ? Quel budget ? Quel gain attendu ? |
| **Pourquoi** ? | Pourquoi ce projet maintenant ? Pourquoi cette approche ? |

### 3.3 La technique des "5 Pourquoi"

Technique issue du Toyota Production System pour identifier les causes racines d'un problème.

**Exemple** :

```
Client : "On veut un modèle de prédiction du churn."

Pourquoi ? → "Parce qu'on perd trop de clients."
Pourquoi ? → "Parce qu'ils partent à la concurrence."
Pourquoi ? → "Parce qu'ils sont insatisfaits du service client."
Pourquoi ? → "Parce que les temps de réponse sont trop longs."
Pourquoi ? → "Parce qu'on manque de personnel aux heures de pointe."
```

**Révélation** : le vrai problème n'est peut-être pas la prédiction du churn, mais l'optimisation des plannings du service client !

>  Attention à ne pas transformer l'entretien en interrogatoire. Les "pourquoi" doivent être posés avec tact et bienveillance.

### 3.4 Questions de clarification

Indispensables pour lever les ambiguïtés :

- "Que voulez-vous dire exactement par... ?"
- "Pouvez-vous me donner un exemple concret ?"
- "Comment cela se traduit-il au quotidien ?"
- "Qu'est-ce qui vous ferait dire que c'est réussi ?"
- "Sur une échelle de 1 à 10, quelle importance accordez-vous à... ?"

### 3.5 Identifier les contraintes

Ne jamais oublier d'explorer les contraintes — elles conditionnent la faisabilité :

| Dimension | Questions types |
|-----------|-----------------|
| **Budget** | "Quelle enveloppe est prévue ?" "Y a-t-il des coûts récurrents acceptables ?" |
| **Délais** | "Pour quand en avez-vous besoin ?" "Y a-t-il une date impérative ?" |
| **Ressources** | "Qui sera disponible côté métier ?" "Quelle implication IT ?" |
| **Données** | "Quelles données existent ?" "Sont-elles accessibles ?" "Quelle qualité ?" |
| **Technique** | "Quelles contraintes d'infrastructure ?" "Quels systèmes existants ?" |
| **Légal** | "Y a-t-il des données sensibles ?" "Quelles contraintes RGPD ?" |

---

## 4. Besoin exprimé vs besoin réel

### 4.1 Le phénomène de l'iceberg

Ce que le client exprime n'est souvent que la partie émergée de l'iceberg :

![Schéma : iceberg des besoins clients](./Images/IcebergBesoinsClient.png)

### 4.2 Pourquoi cet écart ?

Plusieurs raisons expliquent l'écart entre besoin exprimé et besoin réel :

- **Biais de solution** : le client pense déjà savoir ce qu'il veut
- **Vocabulaire limité** : il ne sait pas exprimer son besoin en termes data
- **Contexte politique** : il ne peut pas tout dire
- **Méconnaissance** : il ne sait pas ce qui est possible
- **Habitude** : "on a toujours fait comme ça"

### 4.3 Détecter le vrai besoin

**Signaux d'alerte** (le besoin exprimé n'est probablement pas le vrai) :
- Le client commence par une solution technique : "Je veux du machine learning"
- Le besoin est très vague : "Je veux mieux comprendre mes données"
- Le besoin change au fil de la conversation
- Incohérence entre le problème décrit et la solution demandée

**Techniques pour creuser** :
- "Imaginons que la solution soit en place demain. Qu'est-ce que ça change concrètement pour vous ?"
- "Si vous deviez résoudre ce problème sans aucune technologie, comment feriez-vous ?"
- "Qu'est-ce qui vous empêche de dormir la nuit ?"
- "Qu'est-ce qui se passe si on ne fait rien ?"

### 4.4 Exemple de traduction besoin → problématique data

| Besoin exprimé | Questions à poser | Besoin réel identifié | Problématique data science |
|----------------|-------------------|----------------------|---------------------------|
| "Je veux un dashboard de mes ventes" | Pourquoi ? Qu'allez-vous en faire ? Quelles décisions ? | Anticiper les ruptures de stock | **Prévision de séries temporelles** (forecasting) |
| "Je veux de l'IA pour mes emails" | Quel volume ? Quel problème ? Qu'en faites-vous actuellement ? | Trier automatiquement les réclamations urgentes | **Classification de texte** (NLP) |
| "Je veux connaître mes meilleurs clients" | Pour en faire quoi ? C'est quoi "meilleur" ? | Cibler les actions de fidélisation | **Segmentation** (clustering) ou **scoring** |
| "Je veux prédire le churn" | Pourquoi partent-ils ? Que ferez-vous des prédictions ? | Identifier les clients à risque pour les retenir | **Classification binaire** + analyse des drivers |

---

## 5. Structure d'un entretien de cadrage

### 5.1 Les 5 phases de l'entretien

![Schéma phases entretien](./Images/PhasesEntretien.png)

### 5.2 Phase 1 : Introduction

**Objectifs** : créer un climat de confiance, cadrer l'échange.

**À faire** :
- Se présenter brièvement (parcours, rôle)
- Expliquer l'objectif de l'entretien
- Annoncer la durée et le déroulé
- Demander l'accord pour prendre des notes
- Vérifier qui sont les participants et leur rôle

**Exemple d'amorce** :
> "Bonjour, je suis [nom], data scientist chez [entreprise]. L'objectif de notre échange aujourd'hui est de bien comprendre votre besoin pour évaluer comment nous pourrions vous aider. Je vais vous poser des questions sur votre contexte et vos attentes. Ça devrait durer environ une heure. Je prendrai des notes et vous enverrai un compte-rendu. Est-ce que ça vous convient ?"

### 5.3 Phase 2 : Exploration du contexte

**Objectifs** : comprendre l'environnement métier, les enjeux, l'historique.

**Questions types** :
- "Pouvez-vous me décrire votre activité / votre service ?"
- "Quels sont vos principaux enjeux actuellement ?"
- "Comment fonctionne le processus concerné aujourd'hui ?"
- "Avez-vous déjà essayé des solutions ? Qu'est-ce qui a fonctionné ou non ?"
- "Qui sont les personnes concernées par ce sujet ?"

### 5.4 Phase 3 : Définition des besoins

**Objectifs** : identifier le problème réel, les objectifs, les critères de succès.

**Questions types** :
- "Quel problème cherchez-vous à résoudre ?"
- "Qu'est-ce qui vous ferait dire que le projet est un succès ?"
- "Comment mesurez-vous la situation actuelle ?"
- "Quelles sont vos priorités ? Qu'est-ce qui est non négociable ?"
- "Quelles sont les contraintes (budget, délais, ressources) ?"

**Point critique** : obtenir des critères de succès **mesurables** (penser aux objectifs SMART : Spécifiques, Mesurables, Acceptable, Réalistes, Temporellement définis).

| Critère flou | Critère mesurable |
|--------------|-------------------|
| "Améliorer la satisfaction client" | "Augmenter le NPS de 10 points en 6 mois" |
| "Réduire le churn" | "Passer de 5% à 3% de churn mensuel" |
| "Gagner du temps" | "Réduire le temps de traitement de 2h à 30min" |

### 5.5 Phase 4 : Données et faisabilité

**Objectifs** : évaluer la faisabilité technique, identifier les risques.

**Questions types** :
- "Quelles données avez-vous sur ce sujet ?"
- "Où sont-elles stockées ? Dans quel format ?"
- "Depuis quand les collectez-vous ? Quel historique ?"
- "Qui y a accès ? Y a-t-il des restrictions ?"
- "Quelle est leur qualité ? Y a-t-il des données manquantes ?"
- "Y a-t-il des données sensibles (RGPD) ?"

**Signaux d'alerte** :
- "On a des données quelque part, il faudrait demander à l'IT"
- "Les données sont dans des fichiers Excel sur différents postes"
- "On n'a commencé à collecter ces données que le mois dernier"

### 5.6 Phase 5 : Synthèse et prochaines étapes

**Objectifs** : valider la compréhension, définir la suite.

**À faire** :
- Résumer les points clés (besoin, objectifs, contraintes)
- Faire valider par le client : "Est-ce que j'ai bien compris ?"
- Lister les questions en suspens
- Définir les prochaines étapes concrètes
- Fixer une date pour le prochain point

**Exemple de clôture** :
> "Pour résumer, vous souhaitez [besoin] afin de [objectif], avec comme critère de succès [métrique]. Les principales contraintes sont [contraintes]. Côté données, vous disposez de [données]. Est-ce bien cela ? 
> Pour la suite, je vous propose de [prochaines étapes]. Je vous envoie un compte-rendu d'ici [date]. On se revoit le [date] pour [objectif]."

---

## 6. Gérer les attentes et les situations difficiles

### 6.1 Les attentes irréalistes

**Exemples courants** :
- "Le machine learning peut prédire l'avenir avec certitude"
- "C'est juste un petit algorithme, ça prend 2 jours"
- "On veut 99% de précision"
- "L'IA va remplacer toute l'équipe"

**Comment réagir** :

1. **Ne pas dire non brutalement** — cela braque le client
2. **Accueillir l'attente** — "Je comprends que vous souhaitiez..."
3. **Expliquer la réalité** — avec pédagogie et exemples concrets
4. **Proposer une alternative réaliste** — "Ce qu'on peut faire, c'est..."

**Exemple de reformulation** :
> Client : "Je veux que l'algorithme prévoie exactement combien je vais vendre."
> 
> Vous : "Je comprends le besoin d'avoir une visibilité sur les ventes futures. En revanche, une prédiction 'exacte' n'est pas réaliste — il y aura toujours une marge d'erreur car des facteurs imprévisibles entrent en jeu. Ce qu'on peut vous proposer, c'est un modèle qui donne une fourchette fiable, par exemple 'entre 950 et 1050 unités avec 80% de confiance'. Est-ce que ça répondrait à votre besoin ?"

### 6.2 Le syndrome du marteau

> "Quand on a un marteau, tout ressemble à un clou."

Certains clients arrivent avec une solution en tête (souvent "de l'IA") sans avoir clarifié le problème.

**Exemple** :
> Client : "On veut du deep learning pour notre CRM."
> 
> Vous : "D'accord, et quel problème cherchez-vous à résoudre avec le CRM ?"
> 
> Client : "Euh... on veut l'améliorer."
> 
> Vous : "Améliorer dans quel sens ? Qu'est-ce qui ne fonctionne pas bien aujourd'hui ?"

**Stratégie** : toujours ramener au problème métier avant de parler solution.

### 6.3 Le périmètre qui dérive

Le "scope creep" est l'ennemi de tout projet. Le client ajoute des demandes au fil de l'eau.

**Comment gérer** :
- Documenter le périmètre initial par écrit
- À chaque nouvelle demande : "C'est intéressant. Est-ce que ça remplace quelque chose du périmètre initial ou ça s'ajoute ?"
- Évaluer l'impact : "Si on ajoute ça, il faut soit décaler le délai, soit retirer autre chose"
- Proposer un "parking lot" : liste des idées à traiter dans une phase 2

### 6.4 Le client qui ne sait pas ce qu'il veut

**Signes** :
- Réponses vagues ou contradictoires
- "Je vous fais confiance, vous êtes l'expert"
- Le besoin change à chaque réunion

**Stratégie** :
- Proposer des options concrètes : "On pourrait faire A, B ou C. Voici les avantages et inconvénients de chaque..."
- Utiliser des exemples visuels ou des maquettes
- Faire un mini-POC (proof of concept) rapide pour matérialiser
- Impliquer d'autres parties prenantes

### 6.5 Dire non avec diplomatie

Parfois, il faut refuser — mais toujours avec tact :

| À éviter | À privilégier |
|----------|---------------|
| "C'est impossible" | "C'est très ambitieux dans ce délai. Voici ce qui serait réaliste..." |
| "Vous n'avez pas les données" | "Pour ce type de projet, il nous faudrait [données]. Est-ce que c'est quelque chose qu'on pourrait construire ?" |
| "Ça ne marchera jamais" | "Il y a des risques significatifs sur ce point. Je vous propose qu'on fasse d'abord un test pour valider..." |
| "Ce n'est pas mon job" | "Ce sujet dépasse mon périmètre, mais je peux vous mettre en contact avec..." |

---

## 7. Formaliser les besoins

### 7.1 Le compte-rendu d'entretien

À envoyer **dans les 48h** suivant l'entretien.

**Structure type** :

```
═══════════════════════════════════════════════════════════════════
COMPTE-RENDU D'ENTRETIEN DE CADRAGE
═══════════════════════════════════════════════════════════════════

Date : 
Participants : 
Durée : 
Rédacteur : 

───────────────────────────────────────────────────────────────────
1. CONTEXTE
───────────────────────────────────────────────────────────────────
[Résumé du contexte métier, enjeux, historique]

───────────────────────────────────────────────────────────────────
2. BESOIN EXPRIMÉ
───────────────────────────────────────────────────────────────────
[Ce que le client a demandé initialement]

───────────────────────────────────────────────────────────────────
3. BESOIN CLARIFIÉ
───────────────────────────────────────────────────────────────────
[Le besoin réel identifié après discussion]

───────────────────────────────────────────────────────────────────
4. OBJECTIFS ET CRITÈRES DE SUCCÈS
───────────────────────────────────────────────────────────────────
• Objectif 1 : ... (métrique : ...)
• Objectif 2 : ... (métrique : ...)

───────────────────────────────────────────────────────────────────
5. CONTRAINTES IDENTIFIÉES
───────────────────────────────────────────────────────────────────
• Budget : 
• Délais : 
• Ressources : 
• Données : 
• Technique : 
• Légal/RGPD : 

───────────────────────────────────────────────────────────────────
6. DONNÉES DISPONIBLES
───────────────────────────────────────────────────────────────────
[Sources, volumes, qualité, accessibilité]

───────────────────────────────────────────────────────────────────
7. POINTS EN SUSPENS
───────────────────────────────────────────────────────────────────
• Question 1 : ... (à clarifier avec : ...)
• Question 2 : ...

───────────────────────────────────────────────────────────────────
8. PROCHAINES ÉTAPES
───────────────────────────────────────────────────────────────────
| Action                | Responsable | Échéance |
|-----------------------|-------------|----------|
|                       |             |          |

───────────────────────────────────────────────────────────────────
Prochaine réunion : [date, heure, participants, objectif]
═══════════════════════════════════════════════════════════════════
```

### 7.2 Le document de cadrage (cahier des charges simplifié)

Pour les projets plus conséquents, un document de cadrage formel :

```
═══════════════════════════════════════════════════════════════════
DOCUMENT DE CADRAGE PROJET DATA
═══════════════════════════════════════════════════════════════════

1. INFORMATIONS GÉNÉRALES
   • Nom du projet : 
   • Sponsor : 
   • Chef de projet : 
   • Date de rédaction : 
   • Version : 

2. CONTEXTE ET ENJEUX
   • Contexte business : 
   • Problème à résoudre : 
   • Enjeux / impacts si non résolu : 

3. OBJECTIFS DU PROJET
   • Objectif principal : 
   • Objectifs secondaires : 
   • Ce qui est hors périmètre : 

4. CRITÈRES DE SUCCÈS
   | Critère | Métrique | Valeur actuelle | Valeur cible |
   |---------|----------|-----------------|--------------|
   |         |          |                 |              |

5. PÉRIMÈTRE FONCTIONNEL
   • Fonctionnalités incluses : 
   • Fonctionnalités exclues (phase 2) : 
   • Utilisateurs cibles : 

6. DONNÉES
   • Sources de données : 
   • Volume et historique : 
   • Qualité connue : 
   • Contraintes d'accès : 
   • Données sensibles (RGPD) : 

7. CONTRAINTES
   • Budget : 
   • Délais : 
   • Ressources disponibles : 
   • Contraintes techniques : 
   • Contraintes légales : 

8. RISQUES ET HYPOTHÈSES
   | Risque / Hypothèse | Probabilité | Impact | Mitigation |
   |--------------------|-------------|--------|------------|
   |                    |             |        |            |

9. ORGANISATION
   • Équipe projet : 
   • Gouvernance : 
   • Fréquence des points : 

10. PLANNING PRÉVISIONNEL
    • Phase 1 - Exploration : [dates]
    • Phase 2 - Modélisation : [dates]
    • Phase 3 - Validation : [dates]
    • Phase 4 - Déploiement : [dates]

11. VALIDATION
    | Nom | Rôle | Date | Signature |
    |-----|------|------|-----------|
    |     |      |      |           |
═══════════════════════════════════════════════════════════════════
```

---

## 8. Pièges courants et bonnes pratiques

### 8.1 Les 7 pièges à éviter

| Piège | Pourquoi c'est un problème | Comment l'éviter |
|-------|---------------------------|------------------|
| **Proposer une solution avant de comprendre** | On risque de résoudre le mauvais problème | Toujours commencer par "Quel problème ?" |
| **Utiliser du jargon technique** | Le client décroche, ne comprend pas, n'ose pas dire | Adapter son vocabulaire, vérifier la compréhension |
| **Promettre la lune** | Attentes irréalistes = déception garantie | Être transparent sur les limites et incertitudes |
| **Accepter un périmètre flou** | Scope creep, conflits, projet sans fin | Documenter précisément, faire valider par écrit |
| **Négliger les contraintes** | Solution infaisable ou inutilisable | Explorer systématiquement budget, délais, données, légal |
| **Ne parler qu'aux décideurs** | Passer à côté du besoin réel des utilisateurs | Impliquer les utilisateurs finaux |
| **Ne pas documenter** | "Il avait dit que..." = conflits assurés | Compte-rendu écrit, validé, archivé |

### 8.2 Les 7 bonnes pratiques

| Pratique | Bénéfice |
|----------|----------|
| **Préparer l'entretien** | Montrer du professionnalisme, poser des questions pertinentes |
| **Poser des questions "naïves"** | Éviter les suppositions, clarifier les implicites |
| **Reformuler régulièrement** | Vérifier la compréhension, montrer l'écoute |
| **Être transparent** | Construire la confiance, éviter les mauvaises surprises |
| **Documenter et partager** | Créer une référence commune, éviter les malentendus |
| **Proposer des options** | Impliquer le client, lui donner le contrôle |
| **Conclure par des actions concrètes** | Faire avancer le projet, responsabiliser chacun |

---

## Exercice, ressource A : Grille de questions types

### Contexte et enjeux
- Pouvez-vous me présenter votre activité / votre service ?
- Quels sont vos principaux enjeux actuellement ?
- Qu'est-ce qui vous amène à lancer ce projet maintenant ?

### Problème et objectifs
- Quel problème cherchez-vous à résoudre ?
- Qu'est-ce qui se passe si on ne fait rien ?
- Qu'est-ce qui vous ferait dire que le projet est réussi ?
- Comment mesurez-vous cela aujourd'hui ?

### Processus actuel
- Comment faites-vous actuellement ?
- Combien de temps cela prend-il ?
- Quelles sont les difficultés rencontrées ?
- Avez-vous déjà essayé des solutions ?

### Données
- Quelles données avez-vous sur ce sujet ?
- Où sont-elles ? Qui y a accès ?
- Depuis quand les collectez-vous ?
- Quelle est leur qualité ?

### Contraintes
- Quel est le budget prévu ?
- Pour quand en avez-vous besoin ?
- Qui sera impliqué côté métier / IT ?
- Y a-t-il des contraintes légales (RGPD) ?

### Utilisation
- Qui utilisera la solution ?
- Comment l'utiliseront-ils concrètement ?
- À quelle fréquence ?
- Quelles décisions prendront-ils avec ?

---

## Exercice, ressource B : Grille d'auto-évaluation

| Critère | 1 | 2 | 3 | 4 | Commentaire |
|---------|---|---|---|---|-------------|
| **Écoute active** (reformulation, attention) | | | | | |
| **Qualité des questions** (ouvertes, pertinentes) | | | | | |
| **Identification du besoin réel** | | | | | |
| **Gestion des attentes** (réalisme, diplomatie) | | | | | |
| **Adaptation du discours** | | | | | |
| **Prise de notes** | | | | | |
| **Synthèse et prochaines étapes** | | | | | |
| **Posture professionnelle** | | | | | |

**Échelle** : 1 = À améliorer | 2 = Acceptable | 3 = Bien | 4 = Excellent

**Points forts identifiés** :

**Axes d'amélioration** :

---

## Exercice, ressource C : Scénarios pour jeux de rôle

### Scénario 1 : Retail — Prévision des ventes

**Contexte** : Vous êtes responsable des achats dans une chaîne de supermarchés. Vous gérez les commandes pour 50 magasins.

**Problème** : Vous avez régulièrement des ruptures de stock sur certains produits et du gaspillage sur d'autres. Vous commandez "au feeling" basé sur votre expérience.

**Attente** : Vous avez entendu parler de l'IA et vous voulez "un outil intelligent pour commander".

**Informations à révéler progressivement** :
- Vous avez 3 ans d'historique de ventes dans un ERP
- Les promotions sont décidées 2 semaines à l'avance
- Certains produits sont saisonniers
- Le délai de livraison fournisseur est de 5 jours

**Attente irréaliste à jouer** : "Je veux zéro rupture ET zéro gaspillage"

---

### Scénario 2 : RH — Turnover

**Contexte** : Vous êtes DRH d'une entreprise de 500 personnes dans le secteur tech.

**Problème** : Le turnover a explosé (passé de 10% à 25% en 2 ans). Le recrutement coûte cher et les équipes sont déstabilisées.

**Attente** : Vous voulez "prédire qui va partir" pour agir avant.

**Informations à révéler progressivement** :
- Vous avez les données RH classiques (ancienneté, salaire, poste, manager...)
- Vous faites une enquête de satisfaction annuelle
- Les entretiens annuels sont peu formalisés
- Vous suspectez que les départs sont liés à certains managers

**Attente irréaliste à jouer** : "Je veux savoir avec certitude qui va démissionner dans les 6 mois"

---

### Scénario 3 : Service client — Tri des emails

**Contexte** : Vous dirigez le service client d'une compagnie d'assurance. Votre équipe reçoit 500 emails par jour.

**Problème** : Les emails sont traités dans l'ordre d'arrivée, mais certains sont urgents (sinistres graves) et attendent parfois 48h.

**Attente** : Vous voulez "de l'intelligence artificielle pour trier les emails".

**Informations à révéler progressivement** :
- Les emails arrivent sur une boîte générique
- Vous n'avez pas d'historique étiqueté (pas de classification existante)
- Les agents font un premier tri manuel actuellement
- Il y a environ 10% d'emails vraiment urgents

**Attente irréaliste à jouer** : "L'IA doit comprendre parfaitement chaque email et jamais se tromper sur les urgences
