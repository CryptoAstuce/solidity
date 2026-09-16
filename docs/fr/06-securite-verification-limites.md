# 6. Sécurité, vérification et limites

Le compilateur signale des catégories de problèmes, mais il ne prouve pas qu’un protocole est sûr. Les analyses statiques, le model checker, les tests et la revue humaine couvrent des risques complémentaires.

Les avertissements portent par exemple sur des variables jamais utilisées, des retours ignorés, des constructions ambiguës ou des changements de comportement liés à une version. Les ignorer systématiquement masque le signal utile.

La vérification formelle encode certaines propriétés dans un solveur SMT. Elle dépend du périmètre modélisé et des hypothèses de l’environnement ; une propriété non exprimée n’est pas vérifiée.

Périmètre : ce parcours traduit les composants de parsing, AST, types, ABI, codegen, IR/Yul, optimisation et formal verification présents dans le dépôt. Aucune installation, compilation ou exécution de test n’a été effectuée. Pour vérifier le comportement concret, consulter les suites de tests et les guides officiels du dépôt.

Retour : [sommaire du parcours](README.md).
