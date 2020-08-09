# Yuno.js
This bot is a fork of [Rushnett's starboard](https://github.com/Rushnett/starboard) but modified to fit for **HeavenHell Entertainment** Discord. Bot token login methods are changed since the original starboard is logged in via a config.json file. It has been changed to fit **Heroku Hosting** login configuration variables instead.
![Yuno](https://media.discordapp.net/attachments/718085539173105687/741789185110704138/da8w79t-aae179cc-4265-4da2-808d-a77c8e9661d2.jpg?width=768&height=432)

# Starboard
Starboard (also known as the smugboard™) is a Discordjs bot originally created (and still running) for moonmoon's discord server. It allows users to react to messages on a given server, and pin messages that reach a threshold to a special channel. This implementation is a barebones starboard that can work on one discord server with minimal setup. No databases are required.

## Getting Started
### Requirements
NodeJS >=10.0.0
### Setup
After cloning the repository, the only setup that needs to be done involves creating a `settings.json` file in the config folder. The following is an example of how the file needs to look:
```
{
  "token": "bot_token",
  "serverID": "693277318496920420",
  "channelID": "461248569698208129",
  "reactionEmoji": "⭐",
  "threshold": 15,
  "hexcolor": "00AE86",
  "dateCutoff": 3,
  "fetchLimit": 100
}
```
**token:** the discord bot token you get from your discord [developer portal](https://discordapp.com/developers/applications/).

**serverID:** the ID of the server you want the bot to run in. After enabling developer mode, you can right click the server icon to get the server ID.

**channelID:** the ID of the channel you want the starboard bot to post to. You can right click the channel name and obtain the channel ID after enabling developer mode.

**reactionEmoji:** the emoji you want the bot to listen to. For default emojis, use the literal emoji. To easily obtain this, you can put a `\` infront of any emoji name like `\:star:` in discord (which would create ⭐). For custom emojis, simply put the exact name like `moon2SMUG`.

**threshhold:** the amount of reactions it takes for a message to be posted to the starboard.

**hexcolor:** the color of the embed in hex.

**dateCutoff:** how old a message can be, in days, and still be tracked by the bot. if you don't want really old messages getting posted, then keep this number low.

**fetchLimit:** how many messages from the starboard channel will be loaded in memory. This lets the script know what messages have already been posted. It's recommended to change this with respect to `dateCutoff` and how big your server is. Anything that isn't tracked has the possibility of getting double posted.

### Running the Project
Use `npm install` to download dependencies. Finally, you can run the bot with `npm start`. I recommend using pm2 for continuous uptime.

## License
This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details.
