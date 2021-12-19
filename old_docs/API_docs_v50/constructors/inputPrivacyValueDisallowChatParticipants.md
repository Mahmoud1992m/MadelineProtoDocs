---
title: inputPrivacyValueDisallowChatParticipants
description: Disallow only participants of certain chats
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputPrivacyValueDisallowChatParticipants  
[Back to constructors index](index.md)



Disallow only participants of certain chats

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|chats|Array of [long](../types/long.md) | Yes|Disallowed chat IDs|



### Type: [InputPrivacyRule](../types/InputPrivacyRule.md)


### Example:

```php
$inputPrivacyValueDisallowChatParticipants = ['_' => 'inputPrivacyValueDisallowChatParticipants', 'chats' => [long, long]];
```  


Or, if you're into Lua:

```lua
inputPrivacyValueDisallowChatParticipants={_='inputPrivacyValueDisallowChatParticipants', chats={long}}

```

