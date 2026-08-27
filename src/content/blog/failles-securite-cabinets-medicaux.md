---
title: "5 failles de sécurité courantes dans les cabinets médicaux"
description: "Données patients exposées, postes non verrouillés, Wi-Fi partagé… Les cabinets de santé sont des cibles faciles. Voici comment y remédier."
date: "2025-07-10"
category: "Santé"
lottie: "/lottie/blog-sante.json"
---

## Les cabinets médicaux, cibles sous-estimées

Un cabinet médical manipule chaque jour des centaines de données sensibles : identités, numéros de sécurité sociale, antécédents médicaux, résultats d'examens. Ces données valent cher sur le marché noir — bien plus qu'un simple numéro de carte bancaire.

Pourtant, la majorité des cabinets de santé n'ont aucune mesure de cybersécurité en place. Voici les 5 failles les plus fréquentes que nous rencontrons sur le terrain.

## 1. Mots de passe partagés entre praticiens

Le mot de passe du logiciel de gestion patients est souvent le même pour tout le cabinet. Parfois même noté sur un post-it collé à l'écran. Si un seul compte est compromis, toutes les données patients sont exposées.

**Ce qu'il faut faire** : un compte nominatif par praticien, des mots de passe uniques et robustes, et l'authentification à deux facteurs sur les accès critiques.

## 2. Postes non verrouillés en salle de consultation

Entre deux patients, le poste reste ouvert avec le dossier médical affiché. N'importe qui — patient suivant, personnel de ménage, visiteur — peut voir ou copier des données.

**Ce qu'il faut faire** : verrouillage automatique après 2 minutes d'inactivité, raccourci Windows+L systématique, et sensibilisation de toute l'équipe.

## 3. Réseau Wi-Fi unique pour tout le monde

Patients en salle d'attente, praticiens, secrétariat — tout le monde utilise le même réseau Wi-Fi. Un patient connecté au Wi-Fi peut potentiellement accéder aux ressources internes du cabinet.

**Ce qu'il faut faire** : séparer le réseau en VLANs — un réseau dédié aux postes médicaux, un réseau invités isolé pour les patients. Deux réseaux Wi-Fi distincts, deux niveaux de sécurité.

## 4. Sauvegardes inexistantes ou non testées

Les logiciels de gestion patients stockent tout en local. Si le disque dur lâche ou si un ransomware chiffre les fichiers, les données sont perdues. Et beaucoup de cabinets n'ont jamais testé la restauration de leurs sauvegardes.

**Ce qu'il faut faire** : sauvegardes automatiques quotidiennes, chiffrées, externalisées (pas sur le même réseau), et testées au moins une fois par trimestre.

## 5. Aucune conformité RGPD ni HDS

Le Règlement Général sur la Protection des Données impose des obligations strictes sur le traitement des données de santé. Les Hébergeurs de Données de Santé (HDS) doivent être certifiés. Beaucoup de cabinets stockent des données patients sur des services non conformes sans le savoir.

**Ce qu'il faut faire** : un audit de conformité pour identifier les manquements, choisir des prestataires certifiés HDS, et documenter les traitements de données.

## Conclusion

Ces failles ne sont pas des cas extrêmes — ce sont les situations que nous rencontrons dans la majorité des cabinets que nous auditons. La bonne nouvelle, c'est qu'elles sont toutes corrigeables, souvent rapidement et sans investissement majeur.

Un diagnostic de votre infrastructure permet d'identifier ces risques et de mettre en place les solutions adaptées à votre cabinet.
