---
title: account.getWallPapers
description: Returns a list of available wallpapers.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: account.getWallPapers  
[Back to methods index](index.md)


Returns a list of available wallpapers.

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|hash|Array of [int](../types/int.md) | IDs of previously fetched wallpapers | Optional|


### Return type: [account\_WallPapers](../types/account_WallPapers.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$account_WallPapers = $MadelineProto->account->getWallPapers(['hash' => [int, int], ]);
```

Or, if you're into Lua:

```lua
account_WallPapers = account.getWallPapers({hash={int}, })
```
