# Catroniq - Lampe de statut (HQLSTR)

Firmware [ESPHome](https://esphome.io/) de la [lampe de statut Catroniq](https://catroniq.com/kits/lampe-de-statut/) : un ESP-01 qui pilote 12 DEL WS2811, chacune contrôlable dans Home Assistant.

## Installation

- **Depuis le navigateur** : https://djiesr.github.io/HQLSTR-status-lamp/ (Chrome ou Edge, ESP-01 sur un programmeur USB).
- **Avec ESPHome** : adoptez l'appareil dans le tableau de bord, ou copiez [`status-lamp-esp01.yaml`](status-lamp-esp01.yaml).

## Publication

Chaque push sur `main` compile le firmware et met à jour la page d'installation (branche `gh-pages`). Pensez à augmenter `project.version` dans le YAML avant de pousser.

La mise à jour automatique depuis Home Assistant (`update: http_request`) n'est pas incluse : avec le client HTTPS, le firmware dépasse la moitié de la mémoire d'un ESP-01 de 1 Mo et ne pourrait plus se mettre à jour par Wi-Fi.
