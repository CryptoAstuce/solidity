# 3. ABI, stockage et interface standard

L’ABI décrit comment une application encode un appel et décode une réponse. Pour une fonction, le selector dérive de sa signature ; les paramètres dynamiques suivent des offsets et des zones de données définies par l’ABI.

Le compilateur produit aussi les métadonnées, les signatures de fonctions, les événements et les erreurs personnalisées. Ces artefacts permettent aux bibliothèques et aux explorateurs de comprendre un contrat sans connaître son code source complet.

Le layout de stockage associe les variables à des emplacements EVM. Les valeurs compactes peuvent partager un slot, tandis que les mappings et tableaux dynamiques utilisent des emplacements dérivés. Une modification d’ordre peut donc casser la compatibilité d’un proxy.

Le résultat est une interface, pas une garantie de sécurité : un ABI correct peut encore exposer une logique vulnérable.

Suite : [IR, Yul et génération du bytecode](04-ir-yul-bytecode.md).
