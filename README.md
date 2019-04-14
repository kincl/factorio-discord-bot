# factorio-discord-bot

## Building for linux

```
GOOS=linux GOARCH=amd64 go build -o factorio-discord-bot . 
```

## Getting guildID

For some reason the discordgo library does not have a few API calls that would
let me walk the Bot's guilds looking for names so we need the guildID. Easiest
way is to enable developer mode on your account and then copy the ID.

* https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-

## Creating a Bot

Create a Discord Application and then add a Bot user and copy that bot user's
token. To add that Bot to your guild, go to OAuth2 under Application, select `bot`
and copy the generated URL and paste it into your browser to authorize the
application's bot user for your guild.

* https://discordapp.com/developers/applications/
* https://github.com/jagrosh/MusicBot/wiki/Adding-Your-Bot-To-Your-Server