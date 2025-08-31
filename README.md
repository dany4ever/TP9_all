# TP9_all

Plan 
Abstract

Résumer les expériences réalisées avec PyTorch.

Souligner l’amélioration de performance et la simplification du code par rapport aux implémentations manuelles.

Mentionner la comparaison (from scratch vs PyTorch).

1. Introduction

Importance des réseaux de neurones pour la classification (binaire, multiclasses, caractères Tifinagh).

Motivation de passer de l’implémentation from scratch à PyTorch :

Gestion automatique du gradient.

GPU acceleration.

Code plus lisible et plus modulaire.

2. Materials and Methods
2.1 Jeux de données

XOR (synthetic).

Pima Indians Diabetes (binaire, 768 instances, 8 features).

TP dataset Tifinagh (grayscale, 33 classes, 32×32).

AMHCD (RGB, 25k+ images, 33 classes).

2.2 Architectures

MLP XOR : [2 → 2 → 1], Tanh.

MLP Pima : [8 → 16 → 8 → 1], ReLU, Sigmoid output.

MLP Tifinagh (Grayscale/RGB) : [1024 → 64 → 32 → 33], ReLU + Softmax.

CNN LeNet-5 : Conv → Pooling → FC layers, adapté pour 33 classes.
