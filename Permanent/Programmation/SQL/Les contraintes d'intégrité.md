---
MOOC: "[[Programmation]]"
Langage: SQL
Type: Abstrait
tags: []
---
Les **contraintes d'intégrité** sont [[Définition - relation|des règles que doivent vérifier certains éléments du monde réel. ]]Cette dernière doit être nommée et s'exprime en langage naturel ou par une formule mathématique.
**Exemple :** Pour qu'une candidature soit enregistrée, il faut que le candidat ait l'âge requis pour la formation et que son dossier soit transmis avant la date limite d'inscription à la formation.
**Cela se traduit par :** *CI1* : AgeCandidat <= AgeMinRequis et *CI2* DateDossier ⇐ DateLimiteInsc 