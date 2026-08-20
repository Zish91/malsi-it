---
title: "Active Directory : les erreurs de config qui coûtent cher"
description: "GPO mal appliquées, comptes orphelins, droits trop larges — les pièges classiques d'un AD mal géré."
date: "2025-04-10"
category: "Administration"
lottie: "/lottie/blog-system.json"
---

## Active Directory : le cœur de votre infrastructure Windows

Active Directory (AD) gère les identités, les accès et les politiques de sécurité de votre parc informatique Windows. Quand il est bien configuré, c'est un outil puissant. Quand il ne l'est pas, c'est une bombe à retardement.

## Les erreurs les plus fréquentes

### 1. Comptes orphelins

Des employés partis depuis des mois dont les comptes sont toujours actifs. Chaque compte orphelin est une porte d'entrée potentielle pour un attaquant.

**Bonne pratique** : désactiver immédiatement les comptes au départ d'un collaborateur, puis les supprimer après une période de rétention définie.

### 2. GPO mal appliquées

Les stratégies de groupe (GPO) sont l'outil central de configuration des postes et des utilisateurs. Mais des GPO mal organisées, en conflit ou non appliquées, c'est le chaos : politiques de mots de passe inactives, pare-feu Windows désactivé, scripts de connexion qui ne tournent pas.

**Bonne pratique** : documenter chaque GPO, tester avec `gpresult`, organiser les OU (Organizational Units) de manière logique.

### 3. Tout le monde est admin du domaine

Le groupe "Admins du domaine" devrait contenir 2-3 comptes maximum. Dans la réalité, on trouve souvent 10, 15, voire 20 comptes avec des privilèges maximaux.

**Bonne pratique** : appliquer le modèle de tiering Microsoft, utiliser des comptes d'administration dédiés, jamais les comptes du quotidien.

### 4. Pas de politique de mots de passe fine

La politique de mots de passe par défaut d'AD est souvent trop permissive. Sans Fine-Grained Password Policies, tous les utilisateurs ont les mêmes exigences — du stagiaire au directeur financier.

**Bonne pratique** : des politiques différenciées selon le niveau de sensibilité du compte.

### 5. Aucune supervision

AD génère des logs précieux : connexions échouées, modifications de groupes, élévations de privilèges. Sans supervision, ces signaux d'alerte passent inaperçus.

**Bonne pratique** : centraliser les logs, mettre en place des alertes sur les événements critiques.

## Conclusion

Un audit Active Directory permet d'identifier ces erreurs et de les corriger avant qu'elles ne deviennent des incidents. C'est souvent rapide, peu coûteux, et ça change tout.
