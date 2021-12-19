---
title: messages.checkHistoryImportPeer
description: messages.checkHistoryImportPeer parameters, return type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_checkHistoryImportPeer.html
---
# Method: messages.checkHistoryImportPeer
[Back to methods index](index.md)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|


### Return type: [messages.CheckedHistoryImportPeer](../types/messages.CheckedHistoryImportPeer.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_CheckedHistoryImportPeer = $MadelineProto->messages->checkHistoryImportPeer(['peer' => InputPeer, ]);
```

Or, if you're into Lua:

```lua
messages_CheckedHistoryImportPeer = messages.checkHistoryImportPeer({peer=InputPeer, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|USER_NOT_MUTUAL_CONTACT|The provided user is not a mutual contact|

