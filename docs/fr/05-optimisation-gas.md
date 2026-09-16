# 5. Optimiseur et estimation du gas

L’optimiseur cherche une représentation moins coûteuse ou plus compacte sans changer le comportement observable. Il peut simplifier des expressions, partager des calculs, supprimer du code mort et réorganiser des blocs.

Solidity possède des réglages d’optimisation et un chemin IR/Yul distinct. Le choix influence la taille du bytecode, le coût du déploiement et le gas consommé par les appels.

L’estimateur de gas analyse les chemins possibles et les opérations générées. Une estimation reste dépendante des entrées et de l’état : elle n’est ni une borne universelle ni une garantie qu’une transaction sera acceptée.

Une optimisation agressive ne remplace pas une conception claire. Les effets de bord, les appels externes et les hypothèses sur le stockage doivent rester lisibles pour l’audit.

Suite : [Sécurité, vérification et limites](06-securite-verification-limites.md).
