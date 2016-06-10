Crystallisation Kinetics
=======================

Le fichier CrystallizationKinetics.mphphb est un fichier comsol physics builder.

Il permet d'ajouter une nouvelle physique dans comsol qui résoud en chaque point d'un domaine la cinétique de Nakamura.

Il a été créé avec COMSOL 5.2.

Pour l'installer, il faut aller dans les préférence COMSOL et activer "physics bulder". Ensuite, ajouter le fichier mphphb avec le manager (cf p.20 du manuel).

La physique baptisée ck (pour cristallisation kinetics) résoud l'équadiff :
dalpha / dt = n_avrami * K_nak * G(alpha)
en chaque point.

K_nak est une propriété matériau (qui peut dépendre de T). n_avrami aussi. La function G (avec ses log et ses puissances) est tronquée pour éviter les problèmes numériques.

On peut ajouter un terme de fusion et le calcul de l'exotherme.

Des exemples 1D basique et 2D avec une thermique sont joints.

Enjoy.

Arthur LEVY Juin - 2016