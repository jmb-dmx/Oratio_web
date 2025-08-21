---
title: Politique de confidentialité — Oratio
---

# Politique de confidentialité — Oratio

_Mise à jour : 21 août 2025_

Cette politique décrit comment **Oratio** traite vos données. Nous visons la **transparence** et la **minimisation** des données.

## 1. Données collectées

**Oratio ne collecte, ne stocke ni ne transmet aucune donnée personnelle à nos serveurs.**  
L’app fonctionne **en local** sur vos appareils. Aucune donnée analytique n’est envoyée par défaut.

Selon vos usages, Oratio peut **accéder** (avec votre consentement) à des ressources du système :

- **Bluetooth** : pour **détecter et se connecter** à des périphériques compatibles (ex. minuteur matériel) et **synchroniser** l’affichage du temps en temps réel.  
  - Les identifiants de périphériques sont utilisés **temporairement** pour l’établissement de la connexion et **ne sont pas stockés** au-delà de la session.
- **Réseau local (Bonjour/mDNS)** : pour **découvrir** et **communiquer** avec des appareils Oratio (Master/Slave) sur le même réseau.  
  - Les adresses IP locales sont utilisées en **mémoire volatile** pour la communication directe et ne sont pas transmises à des tiers.

> Oratio **n’accède pas** à vos contacts, photos, localisation, micro ou caméra, sauf si une future fonction l’exige et **uniquement** après consentement explicite.

## 2. Finalités d’utilisation

- Établir et maintenir une **connexion** avec des périphériques ou appareils Oratio (Bluetooth ou réseau local).  
- **Synchroniser** et **afficher** des informations de minuterie entre appareils lors d’événements.

## 3. Conservation

- Les données techniques (ex. identifiants BT, IP locales) sont conservées **uniquement en mémoire** pendant la session et **ne sont pas persistées**.

## 4. Partage

- Aucune donnée n’est partagée avec des tiers.  
- Aucun SDK publicitaire n’est intégré.

## 5. Sécurité

- Les communications sur le réseau local sont limitées à votre **LAN**.  
- Nous recommandons d’utiliser des réseaux protégés par mot de passe et de maintenir vos appareils à jour.

## 6. Vos droits

Pour toute question, demande d’accès/suppression (si applicable), ou assistance, écrivez-nous :  
**Courriel :** djmb2016@gmail.com

## 7. Modifications

Cette politique peut évoluer. Nous mettrons à jour la date ci-dessus et, si nécessaire, nous informerons via les notes de version.

---

## Chaînes d’autorisation (Info.plist)

Exemple conforme pour l’App Store Review (à adapter si besoin) :

- **NSBluetoothAlwaysUsageDescription**  
  > « Oratio utilise le Bluetooth pour détecter et se connecter à vos minuteurs matériels afin de **synchroniser l’affichage du temps en temps réel** pendant vos événements. Par exemple, l’app se connecte à votre module de minuterie pour démarrer/arrêter et suivre le temps. »

- **NSLocalNetworkUsageDescription**  
  > « Oratio utilise le réseau local pour **découvrir et synchroniser** des appareils Oratio (Master/Slave) sur le même réseau pendant vos événements. »

- **NSBonjourServices** (exemple)
  ```xml
  <array>
    <string>_oratio._tcp</string>
  </array>
