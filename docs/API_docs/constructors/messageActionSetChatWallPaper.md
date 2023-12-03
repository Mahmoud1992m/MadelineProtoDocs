---
title: "messageActionSetChatWallPaper"
description: "The wallpaper » of the current chat was changed."
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messageActionSetChatWallPaper  
[Back to constructors index](/API_docs/constructors/index.html)



The [wallpaper »](https://core.telegram.org/api/wallpapers) of the current chat was changed.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|same|[Bool](/API_docs/types/Bool.html) | Optional|
|for\_both|[Bool](/API_docs/types/Bool.html) | Optional|
|wallpaper|[WallPaper](/API_docs/types/WallPaper.html) | Yes|New [wallpaper](https://core.telegram.org/api/wallpapers)|



### Type: [MessageAction](/API_docs/types/MessageAction.html)


### Example:

```
$messageActionSetChatWallPaper = ['_' => 'messageActionSetChatWallPaper', 'same' => Bool, 'for_both' => Bool, 'wallpaper' => WallPaper];
```  
