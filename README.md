Introduction

Cette application est une Todo List développée avec React pour le frontend et NestJS pour le backend, utilisant une base de données MySQL. Elle permet aux utilisateurs de créer, modifier, supprimer et consulter des tâches.

Choix et décisions techniques

1. Sélection des technologies
	•	Frontend : React
J’ai choisi React pour le frontend en raison de sa popularité et de sa capacité à créer des interfaces utilisateur dynamiques et réactives. Sa communauté active et son écosystème riche en font un choix solide pour des applications modernes.
	•	Backend : NestJS
Pour le backend, NestJS a été sélectionné pour sa structure modulaire et sa robustesse. Construit sur Node.js, il offre une architecture bien définie qui facilite le développement de services évolutifs et maintenables.
	•	Base de données : MySQL
J’ai opté pour MySQL en raison de sa fiabilité et de sa compatibilité avec Prisma, l’ORM utilisé dans ce projet. De plus, MySQL est largement adopté et bien documenté, ce qui facilite son intégration et son utilisation.

2. Gestion de l’état dans React

Pour gérer l’état des composants, j’ai utilisé le hook useState de React. Cette approche permet une gestion simple et efficace de l’état local, adaptée aux besoins de l’application.

3. Structure du projet

J’ai structuré le projet de manière à séparer clairement les différentes responsabilités :
	•	Backend
	•	src/: Contient le code source de l’application backend.
	•	tasks/: Module responsable de la gestion des tâches, incluant le contrôleur et le service associés.
	•	app.module.ts: Module principal de l’application.
	•	main.ts: Point d’entrée de l’application.
	•	Frontend
	•	src/: Contient le code source de l’application frontend.
	•	components/: Composants React, y compris TodoPage.tsx pour l’interface principale.
	•	App.tsx: Composant racine de l’application.
	•	index.tsx: Point d’entrée de l’application.

4. Gestion des dépendances

J’ai utilisé Yarn pour la gestion des dépendances en raison de sa rapidité et de son efficacité dans la gestion du cache, ce qui améliore le temps d’installation des packages.

5. Points d’arrêt et défis rencontrés
	•	Gestion des ports
Lors du développement, j’ai rencontré un conflit de ports, le port 3000 étant déjà utilisé par une autre application. Pour résoudre ce problème, j’ai configuré le frontend pour qu’il s’exécute sur le port 3001, évitant ainsi les conflits.
	•	Gestion des dépendances conflictuelles
J’ai rencontré des conflits entre différentes versions de dépendances, notamment avec ESLint. Pour résoudre ce problème, j’ai aligné les versions des packages concernés et ajusté les configurations pour assurer la compatibilité.
	•	Gestion des types avec TypeScript
Des erreurs de typage sont survenues lors de l’utilisation de TypeScript, notamment des types manquants ou incorrects. J’ai résolu ces problèmes en définissant précisément les types attendus et en ajustant le code en conséquence.

Conclusion

Ce projet m’a permis de renforcer mes compétences en développement full-stack, en particulier dans l’intégration de React et NestJS, ainsi que dans la gestion des bases de données avec Prisma et MySQL. Les défis rencontrés ont été autant d’opportunités d’apprentissage, me permettant d’améliorer ma capacité à résoudre des problèmes complexes et à prendre des décisions techniques éclairées.
