# Lampe de statut

La **lampe de statut HQLSTR** de [Catroniq](https://catroniq.com/kits/lampe-de-statut/) affiche d'un coup d'œil l'état de votre maison : 12 DEL contrôlables une par une depuis [Home Assistant](https://www.home-assistant.io/), grâce à [ESPHome](https://esphome.io/). Une porte ouverte, une alarme armée, une laveuse terminée : à chaque capteur sa couleur.

**[Voir le kit et les instructions de montage sur catroniq.com](https://catroniq.com/kits/lampe-de-statut/)**

## Fonctions

- 12 DEL WS2811 adressables, disponibles une par une dans Home Assistant (**status-lamp 01** à **12**)
- Une lumière qui regroupe toutes les DEL, avec un effet d'animation
- Mises à jour par Wi-Fi depuis le tableau de bord ESPHome

## Installation

Installez l'ESP-01 sur un programmeur USB (avec bouton de programmation), branchez-le à votre ordinateur, puis cliquez sur le bouton ci-dessous. Le firmware s'installe directement depuis votre navigateur, puis la page vous demande votre réseau Wi-Fi.

<script type="module" src="https://unpkg.com/esp-web-tools@10.4.0/dist/web/install-button.js?module"></script>
<esp-web-install-button manifest="./manifest.json"></esp-web-install-button>

- Fonctionne avec **Chrome** ou **Edge** sur ordinateur (pas sur Firefox, Safari ni téléphone).
- Si le programmeur n'est pas détecté :
  1. Vérifiez votre câble USB. Plusieurs câbles servent seulement à la recharge et ne transportent pas les données.
  2. Installez le [pilote USB CH340](https://www.wch-ic.com/downloads/CH341SER_EXE.html), puis débranchez et rebranchez le programmeur.
- Si la page ne propose pas de configurer le Wi-Fi, replacez l'ESP-01 sur la lampe : il crée un réseau **status-lamp-…** (mot de passe `12345678`). Connectez-vous-y avec votre téléphone pour choisir votre Wi-Fi.

Une fois la lampe connectée au Wi-Fi, Home Assistant la détecte automatiquement : ouvrez **Paramètres → Appareils et services** et cliquez sur **Configurer** sous ESPHome.

## Mises à jour

Pour installer une nouvelle version, revenez sur cette page avec l'ESP-01 sur son programmeur USB et cliquez de nouveau sur le bouton. Vous pouvez aussi adopter la lampe dans le tableau de bord ESPHome : les mises à jour se font alors par Wi-Fi, sans retirer l'ESP-01.

## Utilisateurs d'ESPHome

Vous pouvez aussi adopter la lampe dans le tableau de bord ESPHome, ou copier le fichier `status-lamp-esp01.yaml` depuis le [dépôt GitHub](https://github.com/djiesr/HQLSTR-status-lamp).

---

[catroniq.com](https://catroniq.com/kits/lampe-de-statut/)
