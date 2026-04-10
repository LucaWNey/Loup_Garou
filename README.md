# 🐺 Loup-Garou - Minecraft Plugin

![Version](https://img.shields.io/badge/Version-1.0-blue.svg)
![Minecraft Version](https://img.shields.io/badge/Minecraft-1.8-brightgreen.svg)
![Java](https://img.shields.io/badge/Java-8%20|%2011%20|%2016+-orange.svg)

**Loup-Garou** est un plugin Minecraft (Spigot/Bukkit) qui recrée fidèlement le célèbre jeu de société "Les Loups-Garous de Thiercelieux" directement en jeu. 

Ce projet a été développé dans le but de fournir une expérience fluide, automatisée et immersive aux joueurs, avec une gestion complète des cycles jour/nuit, des rôles et des canaux de discussion (chat séparé pour les loups).

---

## ✨ Fonctionnalités Principales

* **Gestion de cycle automatisée :** Le plugin gère le passage du jour et de la nuit, avec des timers personnalisables.
* **Système de Chat Dynamique :** Les joueurs morts, les Loups-Garous et les spectateurs possèdent leurs propres canaux de communication isolés (voir `ChatLG`).
* **Distribution aléatoire des rôles :** Attribution équilibrée selon le nombre de joueurs.
* **Interface et Scoreboard :** Affichage clair des informations de la partie (rôle, temps restant, joueurs vivants) via le scoreboard.

### 🎭 Rôles Inclus (Exemples)
| Rôle | Camp | Description |
| :--- | :--- | :--- |
| **Loup-Garou** | 🐺 Loups | Se réveille la nuit pour éliminer un villageois. |
| **Villageois** | 👨‍🌾 Village | Tente de démasquer les loups lors des votes de jour. |
| **Voyante** | 🔮 Village | Peut découvrir le rôle d'un joueur chaque nuit. |
| **[Ajoute tes rôles...]** | [...] | [...] |

---

## 🛠️ Architecture Technique (Pour les développeurs)

Ce plugin a été pensé avec une architecture orientée objet (POO) pour être facilement maintenable et extensible :
* **Événements (`Listener`) :** Utilisation intensive de l'API Bukkit pour intercepter le chat les dégâts et les interactions.
* **Gestion d'états (State Pattern) :** Le déroulement de la partie est géré par différentes phases (Lobby, Nuit, Jour, Vote).
* **Encapsulation des Joueurs :** Création d'un objet "Wrapper" (`PlayerLG`) autour du `Player` Bukkit natif pour stocker les attributs liés à la partie (rôle, état de vie).

---

## 🚀 Installation

1.  Téléchargez la dernière version du plugin dans l'onglet **[Releases]**.
2.  Glissez le fichier jar dans le dossier `/plugins` de votre serveur Minecraft.
4.  Redémarrez le serveur.
5.  Modifiez le fichier `plugins/LoupGarou/config.yml` selon vos préférences et tapez `/reload`.

## 🤝 Contribution

S'agissant d'un projet personnel/portfolio, les *Pull Requests* ne sont pas activement recherchées, mais les retours ou suggestions d'optimisation sont toujours les bienvenus ! N'hésitez pas à ouvrir une **Issue**.

---

*Développé par LucaWNey*
