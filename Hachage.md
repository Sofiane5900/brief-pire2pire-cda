# 2 **Base de données (BDD)**

## 2.1 Hachage

Le **hachage** est un procédé de sécurité utilisé pour protéger les mots de passe sur **pire2pire**. Il permet de **transformer un mot de passe en une suite de caractères incompréhensible et irréversible**, afin qu’il ne soit jamais stocké en clair dans la base de données. Contrairement au chiffrement, qui peut être déchiffré avec une clé, le hachage est conçu pour ne pas être inversé. Une fois un mot de passe haché, il est quasiment impossible de retrouver sa version d’origine.

Lorsqu’un utilisateur crée un compte ou modifie son mot de passe, celui-ci est immédiatement **haché avant d’être stocké**. Ainsi, même si la base de données venait à être compromise, un attaquant ne pourrait pas récupérer directement les mots de passe des utilisateurs. Cette technique est essentielle pour garantir la sécurité des comptes et empêcher les accès non autorisés.

Tous les algorithmes de hachage ne se valent pas. Certains sont aujourd’hui obsolètes et facilement cassables, comme **MD5** ou **SHA-1**, qui ne sont plus recommandés car ils sont trop rapides et vulnérables aux attaques. À la place, des algorithmes plus sécurisés comme **bcrypt, Argon2 ou PBKDF2** sont utilisés. Ces derniers sont conçus pour être **lents et gourmands en ressources**, ce qui complique les attaques par brute force qui testent des millions de combinaisons possibles pour retrouver un mot de passe.

Cependant, un problème se pose avec le hachage simple : si deux utilisateurs choisissent le même mot de passe, ils obtiendront exactement le même résultat haché dans la base de données. Cela peut permettre à un attaquant de repérer facilement des mots de passe communs en comparant les empreintes hachées. Pour éviter ce risque, une solution supplémentaire est utilisée : le **salage**. Cette technique consiste à ajouter une valeur aléatoire au mot de passe avant de le hacher, ce qui sera expliqué dans la section suivante.
