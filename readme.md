# **_🎶 IA Bot_**

IA est un bot Musique utilisant discord.js 12 ainsi que Lavalink pour atteindre une belle qualité !

# 📚 Utilisation

* Complétez le fichier `config.js`

```js
{
    root: ["OWNER ID"], //identifiant du propiétaire du bot
    bot: {
        id: "BOT ID", //identifiant du bot
        token: "BOT TOKEN", //token du bot
        prefix: "i!" //prefix du bot
    },
    opts: {
        color: 0x2f6e93 //couleur des l'embed
    },
    LAVALINK: {
        NODES: [
            { id: 0, host: "localhost", port: 2635, password: "Mypassword" } //modifiez que si vous changez le fichier application.yml 
        ],
        QUEUES: {}
    }
};
}
```

* Téléchargez jdk (java) version 13
* Téléchargez la dernière version de [Lavalink](https://github.com/Frederikam/Lavalink/releases) en jar et placez le fichier dans le dossier `utils/Lavalink`

## 🚀 Démarrer le serveur Lavalink


**Sur Windows** 
* Ouvrez un terminal et faites `cd [redirection du dossier Lavalink]` puis faites entrer
* Tapez `java -jar Lavalink.jar`

**Sur Linux** 
* Faites la commande `cd [redirection du dossier Lavalink]` puis faites entrer
* Si vous utilisez pm2 : `pm2 start java --name="Lavalink" -- -jar Lavalink.jar`

## Pour démarrer le bot

**Sur Windows** 
* Tapez `cd [racine du bot]` puis faites entrer
* Puis faites la commande `node ia --shard` 

**Sur Linux** 
* Tapez `cd [racine du bot]` puis faites entrer
* Si vous utilisez pm2 : `pm2 start ia.js --name="IA-Bot"`

<br>Notes pour pm2 :

```
pm2 start = démarrer le bot
pm2 stop = arrêter le bot
pm2 restart = redémarrer le bot
```
