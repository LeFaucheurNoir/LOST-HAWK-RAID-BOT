# ŁØST • HΛWK

### Assistant Discord — Diablo Immortal 

**Version actuelle : 2.5.19**

ŁØST • HΛWK est un bot Discord privé conçu pour faciliter l'organisation des activités d'un clan Diablo Immortal. Il centralise la gestion des raids, les inscriptions des joueurs, la composition des équipes et les rappels des événements importants.

---

## ⚔️ Gestion des raids et événements

Le bot dispose d'un système complet de création et de gestion des événements.

- Création de raids avec titre, adversaire, date, heure et description.
- Publication automatique des événements sur Discord.
- Inscriptions organisées par classe.
- Prise en charge des personnages avec leur propre pseudo.
- Possibilité d'inscrire plusieurs personnages sur un même événement.
- Limitation du nombre de places par classe.
- Gestion automatique des listes d'attente lorsque les places sont complètes.
- Fermeture et réouverture des inscriptions.
- Modification et suppression des événements.
- Consultation de la liste des raids et de leurs participants.
- Exportation des participants classés par classe.

### Classes prises en charge

| Classe | Classe | 
|---|---|
| 🪓 Barbare | 🩸 Chevalier de sang |
| 🛡️ Croisé | 🏹 Chasseur de démons |
| 🌿 Druide | 👊 Moine |
| 💀 Nécromancien | 🌪️ Tempête |
| 🔮 Sorcier | 😈 Démoniste |

### Gestion des présences

Chaque événement permet aux joueurs de choisir leur statut :

- **Inscrit :** sélection d'une classe et d'un personnage.
- **Pas sûr :** présence incertaine.
- **Absent :** indisponibilité annoncée.
- **Désinscription :** retrait de ses inscriptions.
- **Suppression individuelle :** possibilité de retirer un personnage sans désinscrire les autres.

Les inscriptions sont actualisées directement sur le message Discord de l'événement.

## 🔁 Événements récurrents

Les raids peuvent être configurés pour se répéter automatiquement :

- Aucune répétition.
- Quotidienne.
- Hebdomadaire.
- Mensuelle.

La publication du prochain événement peut être programmée entre 0 et 30 jours avant sa date prévue.

Les événements d'une même série conservent leur configuration de répétition.

## 🛡️ Guerre des ombres

Le bot intègre un système de rappels automatiques pour les Guerres des ombres.

Les notifications sont programmées le jeudi et le samedi :

| Horaire | Notification |
|---|---|
| 18h30 | Début du rappel — 1 heure avant |
| 19h15 | Rappel — 15 minutes avant |
| 19h25 | Rappel — 5 minutes avant |
| 19h30 | Début de la Guerre des ombres |

Les notifications peuvent mentionner automatiquement le rôle dédié.

### Gestion des placements

La commande `/placements` permet de publier directement sur Discord une composition d'équipes provenant du site de gestion des placements.

Fonctionnalités :
- Importation d'un code de placement au format `HTO1`.
- Décodage des données compressées.
- Organisation par catégories et par équipes.
- Affichage des joueurs et de leurs emojis.
- Affichage du nombre total de joueurs placés.
- Publication sous forme d'embed Discord.

## 🏛️ Assemblée et Chambre forte

Le bot automatise également les rappels quotidiens liés à l'Assemblée et à la Chambre forte.

- Notification à **12h00**.
- Notification à **19h00**.
- Envoi d'une image d'annonce.
- Mention automatique du rôle concerné.
- Désactivation des rappels le dimanche.

## 🌐 Intégration avec le site

ŁØST • HΛWK communique avec le site associé au projet.

L'intégration permet notamment :
- L'exportation des personnages inscrits à un raid.
- La génération d'un code de transfert au format `HTR1`.
- L'ouverture du site avec les données du raid préremplies.
- La récupération des placements de Guerre des ombres depuis un code `HTO1`.
- Une liaison avec le système `panel_bridge`.

Site associé : http://lostxhawk.ooguy.com/

## 🧰 Administration et interface Discord

Le bot utilise les fonctionnalités natives de Discord pour proposer une interface interactive.

- Commandes slash.
- Menus déroulants.
- Boutons interactifs.
- Formulaires de saisie.
- Embeds personnalisés.
- Messages privés éphémères pour certaines opérations.
- Contrôle des permissions administratives.
- Synchronisation des commandes Discord.
- Journalisation de certaines actions.
- Notification lors du démarrage du bot avec sa version actuelle.

La gestion des raids dispose notamment d'un panneau interactif permettant de sélectionner un événement et d'effectuer les opérations disponibles.

### Commandes disponibles

| Commande | Fonction |
|---|---|
| `/sync` | Synchronisation des commandes Discord |
| `/raid_create` | Création d'un raid |
| `/raid_list` | Liste des événements enregistrés |
| `/raid_close` | Fermeture ou réouverture des inscriptions |
| `/raid_delete` | Suppression d'un événement |
| `/raid_export` | Exportation des participants par classe |
| `/raid_repetition` | Configuration des répétitions |
| `/gestion_raids` | Ouverture du panneau de gestion |
| `/placements` | Publication des placements de Guerre des ombres |

## 💾 Données et persistance

Les événements sont enregistrés dans un fichier JSON local.

Le système conserve notamment :
- Les informations des événements.
- Les dates et horaires.
- Les créateurs.
- Les inscriptions et les personnages.
- Les listes d'attente.
- Les limites par classe.
- Les paramètres de répétition.
- Les identifiants des messages Discord associés.

Les événements peuvent ainsi être rechargés après un redémarrage du bot. Les interfaces d'inscription existantes sont également réenregistrées.

## 🖥️ Environnement technique

| Composant | Version / technologie |
|---|---|
| Langage | Python 3.12+ |
| Bibliothèque Discord | discord.py 2.7+ |
| API Discord | Discord Application Commands |
| Données | JSON |
| Fuseau horaire | Europe/Paris |
| Intégration externe | GitHub REST API |
| Compression et encodage | Base64, zlib |
| Planification | discord.ext.tasks |
| Interface externe | panel_bridge |

Le projet utilise également des modules internes, notamment `panel_bridge` et `decode_placements`.

---

## 📋 Historique des versions

### Version 2.5.19

- Ajout d'un ping sur le message de sélection de présence.
- Ajout d'un ping à 12h et 19h pour l'Assemblée et la Chambre forte quotidienne, sauf le dimanche.
- Ajout de rappels à 18h30, 19h15, 19h25 et 19h30 pour la Guerre des ombres, le jeudi et le samedi.

---

<sub>ŁØST • HΛWK — Outil privé de gestion et d'organisation communautaire pour Diablo Immortal.</sub>
