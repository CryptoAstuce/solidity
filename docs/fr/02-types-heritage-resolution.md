# 2. Types, héritage et résolution

Après le parsing, Solidity attribue un type à chaque expression. Les types valeur, référence, tableaux, mappings, contrats, fonctions et littéraux n’ont pas les mêmes règles de copie, de mutabilité ou de stockage.

Le compilateur résout les identifiants, les membres et les surcharges. L’héritage linéarisé détermine l’ordre des bases et influence la résolution des appels internes, des variables et des modificateurs.

Les conversions implicites sont limitées pour éviter qu’un changement de type silencieux ne modifie le comportement du contrat. Les conversions explicites restent une responsabilité du développeur.

Les diagnostics produits à cette étape signalent notamment les appels ambigus, les fonctions non implémentées et les incompatibilités de visibilité ou de mutabilité.

Suite : [ABI, stockage et interface standard](03-abi-stockage-interface.md).
