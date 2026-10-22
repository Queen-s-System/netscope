# NetScope

> Un projet évolutif d'analyse réseau et de diagnostic de sécurité informatique.

NetScope est un projet visant à développer progressivement une boîte à outils
destinée à comprendre, examiner et documenter les environnements informatiques.

Le projet commence par une fonctionnalité simple : analyser la configuration
réseau locale d'une machine, interpréter les informations obtenues et produire
un résultat compréhensible.

À long terme, l'objectif est de construire un outil fiable, modulaire et utile
à d'autres personnes, avec la possibilité d'évoluer vers un produit commercial
si les besoins des utilisateurs le justifient.

## État du projet

**Phase actuelle : cadrage et conception.**

Les premières fonctionnalités sont en cours de définition. Le projet ne
constitue pas encore un outil prêt pour une utilisation en production.

Le développement commencera sous Linux avec Bash. Python pourra être introduit
lorsque la complexité des calculs, des traitements de données ou de l'architecture
le justifiera.

## Objectifs

- Développer des compétences solides en systèmes, réseaux et cybersécurité.
- Automatiser des tâches concrètes d'analyse et de diagnostic.
- Comprendre les résultats collectés au lieu de simplement exécuter des commandes.
- Construire des outils modulaires, testables et documentés.
- Produire des rapports utiles aux utilisateurs.
- Faire évoluer progressivement les fonctionnalités selon les besoins identifiés.
- Explorer un positionnement commercial fondé sur des problèmes réels.

## Première version prévue : v0.1

La première version se concentrera sur l'analyse locale en lecture seule.

Fonctionnalités envisagées :

- Identifier les interfaces réseau de la machine.
- Relever les adresses IPv4 et IPv6 disponibles.
- Récupérer les préfixes ou masques réseau.
- Identifier les routes, passerelles et paramètres DNS disponibles.
- Calculer les propriétés IPv4 d'un sous-réseau lorsque les données nécessaires
  sont disponibles.
- Présenter les résultats de manière claire.
- Signaler les informations indisponibles et les erreurs sans inventer de résultats.

La v0.1 ne modifiera pas la configuration réseau et ne lancera pas de scan sur
d'autres machines.

## Évolutions possibles

Les évolutions suivantes sont des pistes à explorer, et non des engagements
de livraison :

1. Export des résultats en TXT, JSON et CSV.
2. Tests automatisés des calculs réseau et des cas particuliers.
3. Comparaison de relevés et historique local.
4. Découverte des hôtes et inventaire des services sur des réseaux autorisés.
5. Analyse de journaux et vérifications de sécurité.
6. Production de rapports d'audit.
7. Packaging simplifié et interface utilisateur éventuelle.

Chaque évolution devra répondre à un besoin identifiable et apporter une valeur
concrète.

## Principes

- **Fiabilité :** vérifier les calculs et distinguer les faits des hypothèses.
- **Transparence :** présenter les limites de l'analyse et les informations
  qui n'ont pas pu être obtenues.
- **Sécurité :** commencer par des opérations en lecture seule.
- **Autorisation :** limiter les analyses actives aux environnements possédés
  ou explicitement autorisés.
- **Confidentialité :** privilégier le traitement local et documenter tout
  transfert éventuel de données.
- **Qualité :** prévoir des tests, une gestion des erreurs et une documentation.
- **Progression :** privilégier des fonctionnalités simples et fiables avant
  d'ajouter de la complexité.

## Utilisateurs potentiels

Les publics à explorer comprennent notamment :

- Les étudiants en réseaux et cybersécurité.
- Les techniciens informatiques.
- Les administrateurs systèmes et réseaux.
- Les consultants en sécurité.
- Les petites entreprises disposant d'une infrastructure informatique.

Ces catégories constituent des hypothèses. Les besoins devront être validés
auprès de véritables utilisateurs.

## Documentation et suivi

- [Vision du projet](docs/vision.md)
- [Issues GitHub](https://github.com/Queen-s-System/netscope/issues)
- [Jalon v0 — Cadrage du projet](https://github.com/Queen-s-System/netscope/milestone/1)

## Licence

Aucune licence n'a encore été choisie. La réutilisation du code ne doit pas
être présumée autorisée avant qu'une licence appropriée soit définie et publiée.

## Langue

La documentation initiale est rédigée en français. Une documentation anglaise
pourra être ajoutée lorsque cela apportera une valeur aux utilisateurs.
