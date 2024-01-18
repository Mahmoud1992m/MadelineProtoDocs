---
title: "messages.getSavedHistory"
description: "messages.getSavedHistory parameters, return type and example"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getSavedHistory.html
---
# Method: messages.getSavedHistory
[Back to methods index](index.html)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](/API_docs/types/InputPeer.html) | Optional|
|offset\_id|[int](/API_docs/types/int.html) | Optional|
|offset\_date|[int](/API_docs/types/int.html) | Optional|
|add\_offset|[int](/API_docs/types/int.html) | Optional|
|limit|[int](/API_docs/types/int.html) | Optional|
|max\_id|[int](/API_docs/types/int.html) | Optional|
|min\_id|[int](/API_docs/types/int.html) | Optional|
|hash|Array of [long](/API_docs/types/long.html) | Optional|


### Return type: [messages.Messages](/API_docs/types/messages.Messages.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_Messages = $MadelineProto->messages->getSavedHistory(peer: $InputPeer, offset_id: $int, offset_date: $int, add_offset: $int, limit: $int, max_id: $int, min_id: $int, hash: [$long, $long], );
```

