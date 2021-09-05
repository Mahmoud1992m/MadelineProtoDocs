---
title: inputPeerPhotoFileLocation
description: Location of profile photo of channel/group/supergroup/user
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputPeerPhotoFileLocation  
[Back to constructors index](index.md)



Location of profile photo of channel/group/supergroup/user

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|big|[Bool](../types/Bool.md) | Optional|Whether to download the high-quality version of the picture|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|The peer whose profile picture should be downloaded|
|photo\_id|[long](../types/long.md) | Yes|



### Type: [InputFileLocation](../types/InputFileLocation.md)


### Example:

```php
$inputPeerPhotoFileLocation = ['_' => 'inputPeerPhotoFileLocation', 'big' => Bool, 'peer' => InputPeer, 'photo_id' => long];
```  


Or, if you're into Lua:

```lua
inputPeerPhotoFileLocation={_='inputPeerPhotoFileLocation', big=Bool, peer=InputPeer, photo_id=long}

```

