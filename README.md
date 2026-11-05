# ŁØST • HΛWK

Bot Discord de gestion des raids, des inscriptions et des événements pour Diablo Immortal.

## Ajouter le bot à son serveur

Aucune installation de logiciel n'est nécessaire. Il suffit d'ajouter le bot à son serveur Discord.

### [➕ Ajouter ŁØST • HΛWK à mon serveur Discord](https://discord.com/oauth2/authorize?client_id=1558792802782019694&permissions=8&integration_type=0&scope=bot)

1. Ouvrez le lien d'invitation. [CLIQUEZ ICI ➕](https://discord.com/oauth2/authorize?client_id=1558792802782019694&permissions=8&integration_type=0&scope=bot)
2. Connectez-vous à votre compte Discord si nécessaire.
3. Sélectionnez le serveur sur lequel vous souhaitez ajouter le bot.
4. Validez les autorisations demandées.
5. Le bot rejoint votre serveur et devient disponible pour ses membres.

*Il faut disposer de la permission « Gérer le serveur » ou être propriétaire du serveur pour pouvoir ajouter le bot.*

## Première configuration

Une fois le bot ajouté, un administrateur doit configurer les différents salons.

### 1. Utiliser `/config`

Dans un salon Discord, saisissez `/config` et sélectionnez la commande ŁØST • HΛWK.

Vous pouvez renseigner les paramètres suivants :

| Paramètre | Utilité |
|---|---|
| `annonces` | Salon des rappels quotidiens pour l'Assemblée et la Chambre forte |
| `gdo` | Salon des rappels de la Guerre des ombres |
| `logs` | Salon qui reçoit les notifications d'inscriptions et de désinscriptions |
| `role_ping` | Rôle mentionné lors des raids et des rappels |
| `assemblee` | Active ou désactive les rappels quotidiens |
| `guerre_ombres` | Active ou désactive les rappels de la Guerre des ombres |

Vous pouvez renseigner plusieurs paramètres en une seule utilisation de `/config`.

Les paramètres non renseignés conservent leur valeur actuelle.

### 2. Vérifier la configuration

Relancez `/config` sans renseigner de paramètre pour afficher la configuration actuelle du serveur.

La réponse est privée : seul l'administrateur qui utilise la commande peut la voir.

## Utiliser le bot

Les commandes sont accessibles directement dans Discord.

Tapez `/` dans la barre de discussion pour afficher les commandes disponibles, puis sélectionnez ŁØST • HΛWK.

### Gestion des raids

| Commande | Description |
|---|---|
| `/raid_create` | Créer un raid |
| `/raid_list` | Afficher les raids disponibles |
| `/raid_close` | Fermer les inscriptions d'un raid |
| `/raid_delete` | Supprimer un raid |
| `/raid_export` | Exporter les informations d'un raid |
| `/raid_repetition` | Gérer les événements répétitifs |
| `/gestion_raids` | Accéder aux outils de gestion des raids |

Les joueurs peuvent utiliser les messages et les interfaces du bot pour s'inscrire aux raids et gérer leur participation.

### Placements

La commande `/placements` permet d'accéder au système de placements des équipes.

Les placements permettent notamment de répartir les joueurs entre les différentes équipes en fonction des places disponibles.

## Rappels automatiques

Une fois les salons configurés, le bot peut envoyer automatiquement les rappels prévus.

### Assemblée et Chambre forte

Les rappels quotidiens sont programmés à :

- 12 h 00
- 19 h 00

Ils sont prévus du lundi au samedi.

### Guerre des ombres

Les rappels sont programmés les jours de Guerre des ombres :

- 18 h 30 : rappel 1 heure avant
- 19 h 15 : rappel 15 minutes avant
- 19 h 25 : rappel 5 minutes avant
- 19 h 30 : début de la guerre

Les rappels sont envoyés dans le salon défini avec le paramètre `gdo`.

## Classes disponibles

Le bot prend en charge les classes suivantes :

- 🪓 Barbare
- 🩸 Chevalier de sang
- 🛡️ Croisé
- 🏹 Chasseur de démons
- 🌿 Druide
- 👊 Moine
- 💀 Nécromancien
- 🌪️ Tempête
- 🔮 Sorcier
- 😈 Démoniste

## Besoin d'aide ?

Si une commande ne s'affiche pas, vérifiez que le bot est bien présent sur le serveur et que les membres disposent de la permission d'utiliser les commandes d'applications.

Si une fonctionnalité ne fonctionne pas, contactez l'équipe responsable du bot.

---

*ŁØST • HΛWK — La gestion de vos raids Diablo Immortal directement sur Discord.*
