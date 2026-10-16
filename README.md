# Déploiement et sécurisation des communications distantes avec OpenVPN et WireGuard

Projet réalisé à l'Institut Supérieur d'Informatique (ISI), année académique 2025-2026. Encadrant : M. NDIAYE.

## Description
Déploiement de deux solutions VPN open source sous Ubuntu pour sécuriser l'accès distant à un réseau privé, puis comparaison de leurs caractéristiques.

## Environnement
VMware Workstation, Ubuntu 24.04 LTS, réseau virtuel.

## Partie 1 : OpenVPN
- Installation d'OpenVPN et d'Easy-RSA
- Création d'une infrastructure à clés publiques (PKI) : autorité de certification, clé et certificat du serveur
- Configuration du serveur et du client, test du tunnel

## Partie 2 : WireGuard
- Génération des clés, configuration de l'interface `wg0` côté serveur et client
- Routage et règle NAT (`PostUp`)
- Validation : `ping` vers Internet à travers le tunnel (`tcpdump`) et capture **Wireshark** montrant le trafic chiffré (« Encrypted Packet »)

## Comparaison
| Critère | OpenVPN | WireGuard |
|---|---|---|
| Architecture | SSL/TLS, complète et configurable | Moderne, simple et légère |
| Configuration | Plusieurs fichiers, certificats | Simple et concise |
| Performances | Bonnes, plus de surcharge | Très bonnes |
| Ressources | Consommation plus importante | Faible consommation |
| Cas d'usage | Configurations avancées | Simplicité et performance |

## Contenu du dépôt
- `docs/RAPPORT_OPENVPN_WIREGUARD.pdf` : rapport complet

## Auteures
Bintou LO et Ndeye Marieme DIALLO
