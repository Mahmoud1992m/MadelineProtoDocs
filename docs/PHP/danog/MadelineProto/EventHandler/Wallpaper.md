---
title: "danog\\MadelineProto\\EventHandler\\Wallpaper: Represents a [wallpaper](https://core.telegram.org/api/wallpapers)."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\EventHandler\Wallpaper`
[Back to index](../../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Represents a [wallpaper](https://core.telegram.org/api/wallpapers).  



## Properties
* `$id`: `int` Identifier
* `$accessHash`: `int` Access hash
* `$creator`: `bool` Whether we created this wallpaper
* `$default`: `bool` Whether this is the default wallpaper
* `$pattern`: `bool` Whether this is a [pattern wallpaper](https://core.telegram.org/api/wallpapers#pattern-wallpapers)
* `$dark`: `bool` Whether this wallpaper should be used in dark mode.
* `$uniqueId`: `string` Unique wallpaper ID, used when generating [wallpaper links](https://core.telegram.org/api/links#wallpaper-links) or [importing wallpaper links](https://core.telegram.org/api/wallpapers).
* `$media`: `danog\MadelineProto\EventHandler\Media\DocumentPhoto` The actual wallpaper
* `$settings`: `?danog\MadelineProto\EventHandler\Wallpaper\WallpaperSettings` Info on how to generate the wallpaper, according to [these instructions](https://core.telegram.org/api/wallpapers).
---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
