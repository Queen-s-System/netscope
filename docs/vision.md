# Vision du projet NetScope

## 1. Contexte

NetScope est un projet personnel de développement d'outils orientés systèmes,
réseaux et cybersécurité.

Il part d'un besoin concret : comprendre les caractéristiques du réseau auquel
une machine est connectée, recueillir les informations disponibles et en tirer
des conclusions utiles.

Le projet ne doit pas rester un simple exercice de programmation. Il a vocation
à évoluer vers une boîte à outils capable de répondre à de véritables besoins,
utilisable par plusieurs personnes et susceptible de devenir un produit commercial.

## 2. Vision à long terme

Construire progressivement une boîte à outils modulaire qui facilite certaines
tâches d'observation, d'analyse, de diagnostic et de vérification de sécurité
des systèmes et réseaux informatiques.

Chaque outil devra avoir une fonction identifiable. Les différents modules
pourront ensuite être améliorés et, lorsque cela sera pertinent, intégrés dans
un ensemble cohérent.

La vision pourra évoluer à mesure que de nouvelles compétences seront acquises,
que des besoins seront découverts et que les premiers utilisateurs donneront
leur avis.

## 3. Objectifs techniques et pédagogiques

Le développement du projet doit permettre de pratiquer progressivement :

- Le scripting Bash.
- L'administration et l'observation de systèmes Linux.
- Les bases des réseaux TCP/IP.
- L'adressage IPv4 et IPv6, les masques et les sous-réseaux.
- L'analyse de routes et de services réseau.
- La programmation Python.
- Le traitement de données et la génération de rapports.
- Les tests automatisés, la documentation et le contrôle de version.
- Les méthodes d'analyse et de vérification en cybersécurité.

Les technologies seront introduites selon les besoins réels du projet plutôt
que toutes en même temps.

## 4. Objectifs produit et commerciaux

NetScope devra progressivement devenir assez fiable et compréhensible pour
qu'une personne autre que son développeur puisse l'installer et l'utiliser.

Le projet devra explorer les questions suivantes :

- À qui l'outil apporte-t-il le plus de valeur ?
- Quelles tâches difficiles ou répétitives peut-il simplifier ?
- Quelles limites rencontrent les outils déjà disponibles ?
- Quelles fonctionnalités sont réellement importantes pour les utilisateurs ?
- Quelle expérience rendrait l'outil accessible sans en masquer les limites ?
- Quelles formes de distribution ou de commercialisation seraient viables ?

Les publics potentiels comprennent les étudiants, les techniciens informatiques,
les administrateurs réseau, les consultants en sécurité et les petites entreprises.

Ces publics ne sont pas encore validés. Le choix d'une cible prioritaire et d'un
modèle économique dépendra des besoins observés, des retours et des essais
auprès d'utilisateurs.

## 5. Première étape : analyse réseau locale

La première version aura un périmètre volontairement limité.

Elle devra collecter les informations réseau locales accessibles, notamment :

- Les interfaces réseau.
- Les adresses IP et les préfixes disponibles.
- Les masques IPv4, lorsqu'ils peuvent être déterminés.
- Les routes et les passerelles.
- Les serveurs DNS configurés, lorsque ces informations sont accessibles.
- Les propriétés calculables des sous-réseaux à partir de données valides.

L'outil devra ensuite présenter les résultats avec des explications simples.

Il devra signaler les données indisponibles et éviter les conclusions non
justifiées. Une machine peut posséder plusieurs interfaces, et les informations
observables varient selon le système et sa configuration.

### Limites de la première version

- Fonctionnement initial sous Linux.
- Développement initial en Bash.
- Analyse locale en lecture seule.
- Aucune modification de la configuration réseau.
- Aucun scan des autres machines.
- Aucune tentative d'exploitation de vulnérabilités.

## 6. Évolution fonctionnelle envisagée

Après validation de la première version, les évolutions pourront comprendre :

1. Des rapports exportables en TXT, JSON et CSV.
2. Des tests couvrant les calculs et les situations particulières.
3. Une analyse plus détaillée des adresses et des routes.
4. La découverte d'hôtes sur des réseaux autorisés.
5. L'inventaire et l'observation de services accessibles.
6. La comparaison de relevés et la détection de changements.
7. L'analyse de journaux et des vérifications de sécurité.
8. Des fonctions de reporting adaptées à des professionnels.
9. Une interface ou un packaging simplifiant l'utilisation.

Cette liste est indicative. Les priorités seront revues en fonction des progrès
techniques et des besoins identifiés.

## 7. Principes de sécurité et de fiabilité

### Autorisation

Toute analyse active devra être limitée aux systèmes et réseaux que l'utilisateur
possède ou pour lesquels il dispose d'une autorisation explicite.

### Lecture seule par défaut

Les premières versions privilégieront la collecte et l'analyse d'informations
sans modifier la configuration des systèmes examinés.

### Résultats vérifiables

L'outil devra distinguer les données directement observées, les résultats
calculés et les interprétations. Il devra expliquer les limites pertinentes.

### Confidentialité

Les données collectées devront être traitées avec prudence. Leur enregistrement,
leur export et leur éventuelle transmission devront être explicités.

### Qualité logicielle

Le projet devra développer progressivement des tests, une gestion des erreurs,
des instructions d'installation et une documentation permettant la reproduction
des résultats.

## 8. Principes de développement

- Commencer par un problème concret et limité.
- Comprendre les commandes et les mécanismes utilisés.
- Éviter de réécrire inutilement des outils existants.
- Tester les résultats avant d'ajouter de nouvelles fonctionnalités.
- Documenter les décisions techniques importantes.
- Utiliser GitHub pour suivre les tâches, les versions et les changements.
- Réévaluer régulièrement les besoins des utilisateurs.
- Garder le code maintenable et les modules aussi indépendants que possible.

## 9. Critère général de réussite

À terme, NetScope devra être plus qu'une collection de scripts fonctionnant
uniquement sur la machine de son développeur.

Le projet devra fournir une utilisation documentée, des résultats vérifiables,
des limites clairement expliquées et un fonctionnement reproductible.

Sa valeur commerciale devra être évaluée à partir de l'utilité réelle pour
d'autres personnes, de leur retour d'expérience et de leur volonté éventuelle
d'adopter ou de payer pour une solution adaptée à leurs besoins.

## 10. Statut de cette vision

Ce document constitue une première direction de travail, et non un cahier des
charges définitif.

La vision sera mise à jour au fil des apprentissages, des expérimentations,
des retours utilisateurs et des décisions prises dans les issues du projet.
