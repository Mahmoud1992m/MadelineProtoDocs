---
title: help.support
description: Info on support user.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: help.support  
[Back to constructors index](index.md)



Info on support user.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|phone\_number|[string](../types/string.md) | Yes|Phone number|
|user|[User](../types/User.md) | Optional|User|



### Type: [help\_Support](../types/help_Support.md)


### Example:

```php
$help_support = ['_' => 'help.support', 'phone_number' => 'string', 'user' => User];
```  


Or, if you're into Lua:

```lua
help_support={_='help.support', phone_number='string', user=User}

```

