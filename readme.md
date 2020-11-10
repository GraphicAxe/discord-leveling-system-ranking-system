## Discord-Leveling-system-Ranking-system

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Tomato6966/)
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://GitHub.com/Tomato6966/Ask-Me-Anything)
[![Support Server](https://img.shields.io/discord/591914197219016707.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/fS6qBSm)

A easy to setup and easy to use ranking system, and clean interfase using canvacord, using enmap for the database.

## Installation | How to use the Bot

 **1.** Install [node.js v12](https://nodejs.org/api/cli.html#cli_unhandled_rejections_mode) or higher
 **1.1** Install [python 3.9](https://www.python.org/downloads/) or higher
 
 **2.** Download this repo and unzip it    |    or git clone it
 
 **3.** Install all of the packages with **`npm install`**     |  the packages are   **`npm install node.js discord.js enmap canvacord`**
 
 **4.** start the bot with **`node index.js`**

 **NOTE** you can also use **`setup.bat`** and afterwards **`run.bat`** to install packages and run the bot

## Usage - index.js

```javascript
const Discord = require("discord.js");         //load the Discord.js Library
const client = new Discord.Client();           //make a new Client
const config = require("./config.json");       //load the config.json file
const Enmap = require("enmap")                 //load the enmap library
const canvacord = require("canvacord")         //load the canvacord library
client.points = new Enmap({ name: "points" }); //For ranking system
client.on("ready", ()=>console.log("READY"));  //log when the bot gets ready
const leveling = require("./ranking");         //load the leveling file
leveling(client);                              //call the leveling file with the client
client.login(config.TOKEN);                    //start the bot with the bot token
//Coded by Tomato#6966
```

## How it looks like!

![](https://cdn.discordapp.com/attachments/751863584681885777/775632780057903124/RankCard.png)


## **NOTE:**

*If you are having errors/problems with starting delete the package.json file and do, before you install the packages `npm init`*

## SUPPORT ME

You can always Support me by inviting one of my **own Discord Bots**

[![Musicium Music Bot](https://cdn.discordapp.com/attachments/742446682381221938/770055673965707264/test1.png)](https://bit.ly/Musicium)
[![Milrato Muslti Bot](https://cdn.discordapp.com/attachments/742446682381221938/770056826724679680/test1.png)](https://bit.ly/Milrato)

[| fork my repository  |](https://github.com/user/repository/fork)
[watch this repo  |](https://github.com/user/repository/subscription)
[create issue |](https://github.com/user/repository/issues/new)

*Both bots are still in Development, and will always be in development, this means always uptodate and always online and always improving!*
