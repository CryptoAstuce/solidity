# 1. Du texte source à l’AST

Le compilateur Solidity reçoit des unités de source, résout leurs imports puis transforme les caractères en tokens. Le parseur construit un arbre syntaxique abstrait qui représente les contrats, fonctions, déclarations, expressions et annotations NatSpec.

Cette séparation permet de distinguer une erreur de syntaxe d’une erreur de sens. L’AST devient ensuite l’entrée des analyses de type, de la résolution des noms et de la génération des artefacts.

Le dépôt organise ces responsabilités dans libsolidity/parsing et libsolidity/ast. Le CompilerStack coordonne les étapes et conserve les résultats associés à chaque source.

La version du langage indiquée par pragma ne compile pas le contrat elle-même : elle contraint la compatibilité du compilateur sélectionné.

Suite : [Types, héritage et résolution](02-types-heritage-resolution.md).
