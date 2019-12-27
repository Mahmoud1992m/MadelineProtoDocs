---
title: help.setBotUpdatesStatus
description: Informs the server about the number of pending bot updates if they haven't been processed for a long time; for bots only
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: help.setBotUpdatesStatus  
[Back to methods index](index.md)


Informs the server about the number of pending bot updates if they haven't been processed for a long time; for bots only

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|pending\_updates\_count|[int](../types/int.md) | Number of pending updates | Yes|
|message|[string](../types/string.md) | Error message, if present | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->help->setBotUpdatesStatus(['pending_updates_count' => int, 'message' => 'string', ]);
```

Or, if you're into Lua:

```lua
Bool = help.setBotUpdatesStatus({pending_updates_count=int, message='string', })
```


## Return value 

If the length of the provided message is bigger than 4096, the message will be split in chunks and the method will be called multiple times, with the same parameters (except for the message), and an array of [Bool](../types/Bool.md) will be returned instead.

