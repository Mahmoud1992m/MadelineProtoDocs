---
title: "danog\\MadelineProto\\EventHandler\\BotCommands: The [command set](https://core.telegram.org/api/bots/commands) of a certain bot in a certain chat has changed."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\EventHandler\BotCommands`
[Back to index](../../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

The [command set](https://core.telegram.org/api/bots/commands) of a certain bot in a certain chat has changed.  



## Properties
* `$botId`: `int` ID of the bot that changed its command set.
* `$chatId`: `int` The affected chat.
* `$commands`: `list<Command>` New bot commands.
---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
