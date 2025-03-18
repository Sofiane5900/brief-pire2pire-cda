## 1.3 RBAC (Role-Based Access Control)

Sur **pire2pire**, la gestion des accès repose sur le **RBAC (Role-Based Access Control)**, un modèle de contrôle d’accès basé sur les rôles. Ce système permet d’attribuer des permissions aux utilisateurs en fonction de leur rôle au sein de la plateforme, plutôt que d’accorder des droits individuellement à chaque utilisateur. Cette approche facilite la gestion des accès, renforce la sécurité et évite les erreurs humaines liées à une attribution manuelle des permissions.

L’objectif du RBAC est de garantir que **chaque utilisateur possède uniquement les droits nécessaires pour effectuer ses tâches**, tout en empêchant l’accès à des ressources qui ne relèvent pas de son rôle. En structurant les accès selon des rôles bien définis, pire2pire s’assure que les utilisateurs interagissent uniquement avec les fonctionnalités qui leur sont destinées, réduisant ainsi les risques de mauvaise manipulation, d’abus ou de compromission de la plateforme.


---

Trois principaux rôles ont été définis sur pire2pire :



* **Les administrateurs** ont un accès complet à la plateforme. Ils peuvent gérer les utilisateurs, modifier les paramètres du site, administrer les bases de données et assurer la maintenance globale. Ce sont les seuls à disposer de permissions leur permettant de modifier l’architecture du site et d’intervenir sur l’ensemble des fonctionnalités.
* **Les formateurs** disposent de droits leur permettant de créer, modifier et gérer leurs propres cours ainsi que les apprenants qui y sont inscrits. En revanche, ils n’ont pas accès aux paramètres critiques du site ni à la gestion des autres utilisateurs.
* **Les apprenants** ont les permissions les plus restreintes. Leur rôle est uniquement de consulter les formations auxquelles ils sont inscrits et d’interagir avec les contenus pédagogiques. Ils ne peuvent pas modifier des cours, ni accéder aux informations des autres utilisateurs.

L’un des principaux avantages du **RBAC** est qu’il permet une gestion des accès **modulaire et évolutive**. Si pire2pire devait ajouter de nouveaux profils d’utilisateurs (modérateurs, assistants pédagogiques, support technique), il suffirait de leur attribuer un rôle avec des permissions spécifiques, sans devoir ajuster manuellement les droits de chaque utilisateur. Cette flexibilité permet d’adapter le système aux besoins de la plateforme sans compromettre la sécurité.

Grâce au RBAC, pire2pire assure une organisation claire et efficace des droits d’accès, tout en maintenant un contrôle strict sur l’utilisation des fonctionnalités du site. En évitant les accès excessifs et en attribuant des permissions adaptées à chaque rôle, la plateforme garantit une expérience fluide et sécurisée pour ses utilisateurs, tout en simplifiant l’administration des droits et la gestion des accès.
