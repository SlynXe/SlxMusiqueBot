# SlxMusiqueBot
Un bot de musique pour Discord, développé en Node.js par 'SlynXe

## Prérequis
- [Node.js](https://nodejs.org/) (v14 ou plus récent)
- [npm](https://www.npmjs.com/) (normalement inclus avec Node.js)
- Un token de bot Discord (vous pouvez créer un bot sur le [Portail des développeurs Discord](https://discord.com/developers/applications))

## Installation
Suivez les étapes ci-dessous pour installer et configurer votre bot de musique.

### 1. Cloner le dépôt
Clonez ce dépôt sur votre machine locale en utilisant git :

```bash
git clone https://github.com/ItzSlynXe/SlxMusiqueBot.git
cd SlxMusiqueBot
```

### 2. Installer les dépendances
Installez les modules Node nécessaires avec npm :

```bash
npm install
```

### 3. Configurer le bot
Ouvrez le fichier `config.json` et modifiez-le pour inclure votre token de bot Discord et d'autres configurations nécessaires :

```
module.exports = {
    clients: {
        token: 'TON_TOKEN_DISCORD',
        prefix: 'TON_PREFIX',
        activity: '',
        name: 'TON_FOOTER',
        logo: 'TON_LOGO',
        embedColor: 'Red'
    },

    opt: {
        DJ: {
            enabled: false,
            roleName: '🎵︲Musique',
            commands: ['back', 'clear', 'filter', 'loop', 'pause', 'resume', 'seek', 'shuffle', 'skip', 'stop', 'volume']
        },
        maxVol: 100,
        loopMessage: true,
        discordPlayer: {
            ytdlOptions: {
                quality: 'highestaudio',
                highWaterMark: 1 << 25
            }
        }
    }
};
```

- **token** : Remplacez `TON_TOKEN_DISCORD` par le token de votre bot Discord.
- **prefix** : Définissez le préfixe des commandes que vous souhaitez utiliser (par exemple, `!`).

### 4. Démarrer le bot
Utilisez le fichier `start.bat` pour démarrer votre bot facilement sous Windows :

```bash
start.bat
```

Si vous utilisez un autre système d'exploitation, vous pouvez démarrer le bot avec la commande suivante :

```bash
node index.js
```

## Utilisation
Une fois que le bot est en ligne, vous pouvez utiliser les commandes suivantes dans votre serveur Discord :

### ⚙️ Outils
- `ban` : Banni l'utilisateur @ping du serveur..
- `clear` : Nettoie les messages du salon.
- `help` : Affiche les commandes.
- `invite` : Affiche le lien afin de l'inviter.
- `ping` : Affiche le ping.

### 🔊 Musique
- `back` : Retourne en arrière dans la file d'attente.
- `clearmusique` : Supprime la file d'attente.
- `jump` : Passe une musique.
- `nowplaying` : Affiche la musique en cours de lecture.
- `pause` : Met en pause la musique en cours de lecture.
- `play` : Joue une musique.
- `resume` : Reprise la musique en cours de lecture.
- `shuffle` : Mélange la file d'attente.
- `skip` : Passe à la musique suivante dans la file d'attente.
- `stop` : Arrête la musique.
- `volume` : Modifie le volume de la musique.

## Contribuer
Les contributions sont les bienvenues ! Pour signaler des bugs ou proposer des améliorations, veuillez ouvrir une issue ou soumettre une pull request.

## Remerciements
Merci à tous ceux qui contribuent à l'amélioration de ce projet !

Made with 💖 by 'SlynXe
