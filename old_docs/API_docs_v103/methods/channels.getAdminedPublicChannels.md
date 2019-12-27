---
title: channels.getAdminedPublicChannels
description: Get [channels/supergroups/geogroups](https://core.telegram.org/api/channel) we're admin in. Usually called when the user exceeds the [limit](../constructors/config.md) for owned public [channels/supergroups/geogroups](https://core.telegram.org/api/channel), and the user is given the choice to remove one of his channels/supergroups/geogroups.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: channels.getAdminedPublicChannels  
[Back to methods index](index.md)


Get [channels/supergroups/geogroups](https://core.telegram.org/api/channel) we're admin in. Usually called when the user exceeds the [limit](../constructors/config.md) for owned public [channels/supergroups/geogroups](https://core.telegram.org/api/channel), and the user is given the choice to remove one of his channels/supergroups/geogroups.

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|by\_location|[Bool](../types/Bool.md) | Get geogroups | Optional|
|check\_limit|[Bool](../types/Bool.md) | If set and the user has reached the limit of owned public [channels/supergroups/geogroups](https://core.telegram.org/api/channel), instead of returning the channel list one of the specified [errors](#possible-errors) will be returned.<br>Useful to check if a new public channel can indeed be created, even before asking the user to enter a channel username to use in [channels.checkUsername](../methods/channels.checkUsername.md)/[channels.updateUsername](../methods/channels.updateUsername.md). | Optional|


### Return type: [messages\_Chats](../types/messages_Chats.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_Chats = $MadelineProto->channels->getAdminedPublicChannels(['by_location' => Bool, 'check_limit' => Bool, ]);
```

Or, if you're into Lua:

```lua
messages_Chats = channels.getAdminedPublicChannels({by_location=Bool, check_limit=Bool, })
```
