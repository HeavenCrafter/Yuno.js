# Yuno.js

[![Run on Repl.it](https://repl.it/badge/github/HeavenCrafter/Yuno.js)](https://repl.it/github/HeavenCrafter/Yuno.js)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=alert_status)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=bugs)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)
[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=HeavenCrafter_Futaba.js&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=HeavenCrafter_Futaba.js)


This bot is a fork of [Rushnett's starboard](https://github.com/Rushnett/starboard) but modified to fit for **HeavenHell Entertainment** Discord. Bot token login methods are changed since the original starboard is logged in via a config.json file. It has been changed to use .env files usage instead of a config.json format.

![Yuno](https://media.discordapp.net/attachments/718085539173105687/741789185110704138/da8w79t-aae179cc-4265-4da2-808d-a77c8e9661d2.jpg?width=768&height=432)

# Starboard
Starboard (also known as the smugboard™) is a Discordjs bot originally created (and still running) for moonmoon's discord server. It allows users to react to messages on a given server, and pin messages that reach a threshold to a special channel. This implementation is a barebones starboard that can work on one discord server with minimal setup. No databases are required.

### Requirements
NodeJS >=10.0.0

## License
This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details.

## Hosting Platforms
**Heroku and Repl.it**

**Yes, Yuno.js and Futaba.js can be ran on Repl.it and Heroku without much effort.**
I've already went ahead and made 2 files that fits in for both hosting platforms which is -

> Procfile

> .env

**[Heroku]** The `Procfile` file is specifically made for **Heroku** as it is a worker/startup script for Heroku hosting. You can disable the one that came included by default on Heroku and use the one thats made on Yuno.js

**[Repl.it]** The `.env` file is specifically made for **Repl.it**. Unlike Heroku, Repl.it **DOES NOT** come with a built in .env saving proccess or any sort of config .env variable section, only Heroku has that. Which is why I've already went ahead and installed dotenv npm package just in case if you ever want to use these platforms. You can simply just replace the details in the .env file with what you need.

**IMPORTANT**. Remember, if you're going to use Repl.it, MAKE SURE TO **NOT DELETED** THE .ENV FILE. IT IS ABSOLUTELY NEEDED OR YOUR TOKEN WILL BE SHOWN OUT TO THE PUBLIC.
