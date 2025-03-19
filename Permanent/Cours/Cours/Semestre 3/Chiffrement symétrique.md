---
MOOC: "[[Cours]]"
Ressource: "R3.09 : Cryptographie"
Cours: 
Date: 
tags: 
Complete: false
Learned: false
---
**Chiffrement par blocs** = Sys de déchiffrement dans lequel le message clair est découpé en blocs d'une taille fixe, et chacun de ces blocs est chiffré
La longueur $n$ des blocset la taille I des clés sont deux caractéristiques des systèmes de chiffrement par blocs. Le message
Technique de bourrage

## Chiffrement itératif
Tous les systèmes de chiffrement par blocs actuels suivent le schéma suivant :
shcéma

Le bloc $m$ est transformé $r$ fois successivement à l'aide d'une fonction $f$ qui dépend d'uns sous-clé $k_i$. Le message chiffré $c$ est le résultat de la dernière transformation
Le message $m$ est découpé en blocs de $n$ bits :
⇒ $m$ = $m_1m_2...m_k$
Et si la longueur du message n'est pas un multiple de la longueurd'un bloc, on le complète par bourrage

## Le DES
⇒ Date Encryption Standard
- Blocs de 64 bits et une clé de longueur 56 bits avec 16 rounds
- Conçu au début des années 1970
- Standard de chiffrement aux USA de 1977 à 2000


## Objectifs des modes opératoires
Ils doivents masquer les blocs clairs identiques et deux messages identiques chiffrés avec les mêmes clés ne donnent pas les mêmes résultats

>[!info]
>Cela ne fonctionne que pour le chiffrement par blocs

### Le mode ECB
**Chiffrement :** Chaque bloc chiffré $m_i$ est chiffré indépendemment et donne un bloc chiffré  $c_i=E_k(m_i)$
**Déchiffrement :** chaque chiffré est d´echiffr´e ind´ependamment pour donner le clair correspondant
...

### Le mode CBC
**Chiffrement** : un vecteur d’initialisation $IV$ est généré aléatoirement. $ci = Ek (mi ⊕ ci−1)$. Le vecteur $IV$ est transmis avec les blocs chiffrés
**Déchiffrement :** $m_i=D_k(c_i)⊕c_{i-1}$
**Conséquence :** deux blocs clairs identiques chiffrés différemment

### Le mode CFB
**Chiffrement :** Un vecteur d'initialisation $IV$ est généré aléatoirement. $c_i=r_i⊕m_i$ où $r_1=E_k(IV)$ et pour $i>=2$, $r_1=E_k(m_{i-1}⊕r_{i-1})$
**Déchiffrement :** $m_i=c_i⊕r_i$
**Conséquence :** Deux blocs clairs identiques chiffrés indépendemment

### Le mode CTR
**Chiffrement :** $c_i=r_i⊕m_i$, où $r_1=E_k(cpt)$ et pour $i>=2$, $r_i=E_k(cpt+i-1)$
**Déchiffrement :** $m_i=c_i⊕r_i$
**Conséquence :** Deux blocs clairs identiques chiffrés indépendemment

---
# Cours 2


**Prérequis :** [[Le PGCD]], [[Tableau d'Euclide Bézout]], [[Calcul modulaire]] [[Théorème d'Euler]] et 
[[Petit théorème de Fermat]]

---

**Exercices :** [[TD arithmétique]] et [[TD2Arithmetique.pdf]]

---
[[Classes de congruence module n]]
[[Addition, soustraction et multiplication modulo n]]

---

[[Chiffrement affine]]
[[Générateur]]
[[Problème du logarithme discret]]


---
[[Le chiffrement RSA]]

---
