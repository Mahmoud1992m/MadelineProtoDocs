---
title: messages.affectedHistory
description: Affected part of communication history with the user or in a chat.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messages.affectedHistory  
[Back to constructors index](index.md)



Affected part of communication history with the user or in a chat.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|pts|[int](../types/int.md) | Yes|Number of events occured in a text box|
|pts\_count|[int](../types/int.md) | Yes|Number of affected events|
|offset|[int](../types/int.md) | Yes|If a parameter contains positive value, it is necessary to repeat the method call using the given value; during the proceeding of all the history the value itself shall gradually decrease|



### Type: [messages\_AffectedHistory](../types/messages_AffectedHistory.md)


### Example:

```php
$messages_affectedHistory = ['_' => 'messages.affectedHistory', 'pts' => int, 'pts_count' => int, 'offset' => int];
```  


Or, if you're into Lua:

```lua
messages_affectedHistory={_='messages.affectedHistory', pts=int, pts_count=int, offset=int}

```

