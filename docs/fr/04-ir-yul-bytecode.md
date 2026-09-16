# 4. IR, Yul et génération du bytecode

Solidity peut abaisser certaines constructions vers une représentation intermédiaire puis vers Yul. Cette étape rend les transformations plus uniformes entre les contrats et donne à l’optimiseur une vue structurée du programme.

Le codegen traduit ensuite les fonctions, contrôles, accès mémoire, accès stockage, appels et retours en opérations compatibles avec l’EVM. Le bytecode de création contient la logique d’installation ; le runtime bytecode reste sur la chaîne après le déploiement.

Les appels externes passent par le protocole ABI, tandis que les appels internes peuvent être traités comme des sauts dans le même contexte. La différence est déterminante pour msg.sender, msg.value et la gestion du gas.

Les métadonnées et la source map relient les instructions générées au code source, ce qui facilite le débogage sans modifier la sémantique d’exécution.

Suite : [Optimiseur et estimation du gas](05-optimisation-gas.md).
