---
title: "userFull"
description: "Extended user info"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: userFull  
[Back to constructors index](/API_docs/constructors/index.html)



Extended user info

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|blocked|[Bool](/API_docs/types/Bool.html) | Optional|Whether you have blocked this user|
|phone\_calls\_available|[Bool](/API_docs/types/Bool.html) | Optional|Whether this user can make VoIP calls|
|phone\_calls\_private|[Bool](/API_docs/types/Bool.html) | Optional|Whether this user's privacy settings allow you to call them|
|can\_pin\_message|[Bool](/API_docs/types/Bool.html) | Optional|Whether you can pin messages in the chat with this user, you can do this only for a chat with yourself|
|has\_scheduled|[Bool](/API_docs/types/Bool.html) | Optional|Whether [scheduled messages](https://core.telegram.org/api/scheduled-messages) are available|
|video\_calls\_available|[Bool](/API_docs/types/Bool.html) | Optional|Whether the user can receive video calls|
|voice\_messages\_forbidden|[Bool](/API_docs/types/Bool.html) | Optional|Whether this user doesn't allow sending voice messages in a private chat with them|
|translations\_disabled|[Bool](/API_docs/types/Bool.html) | Optional|Whether the [real-time chat translation popup](https://core.telegram.org/api/translation) should be hidden.|
|stories\_pinned\_available|[Bool](/API_docs/types/Bool.html) | Optional|
|blocked\_my\_stories\_from|[Bool](/API_docs/types/Bool.html) | Optional|
|wallpaper\_overridden|[Bool](/API_docs/types/Bool.html) | Optional|
|contact\_require\_premium|[Bool](/API_docs/types/Bool.html) | Optional|
|read\_dates\_private|[Bool](/API_docs/types/Bool.html) | Optional|
|id|[long](/API_docs/types/long.html) | Yes|User ID|
|about|[string](/API_docs/types/string.html) | Optional|Bio of the user|
|settings|[PeerSettings](/API_docs/types/PeerSettings.html) | Yes|Peer settings|
|personal\_photo|[Photo](/API_docs/types/Photo.html) | Optional|Personal profile photo, to be shown instead of `profile_photo`.|
|profile\_photo|[Photo](/API_docs/types/Photo.html) | Optional|Profile photo|
|fallback\_photo|[Photo](/API_docs/types/Photo.html) | Optional|Fallback profile photo, displayed if no photo is present in `profile_photo` or `personal_photo`, due to privacy settings.|
|notify\_settings|[PeerNotifySettings](/API_docs/types/PeerNotifySettings.html) | Yes|Notification settings|
|bot\_info|[BotInfo](/API_docs/types/BotInfo.html) | Optional|For bots, info about the bot (bot commands, etc)|
|pinned\_msg\_id|[int](/API_docs/types/int.html) | Optional|Message ID of the last [pinned message](https://core.telegram.org/api/pin)|
|common\_chats\_count|[int](/API_docs/types/int.html) | Yes|Chats in common with this user|
|folder\_id|[int](/API_docs/types/int.html) | Optional|[Peer folder ID, for more info click here](https://core.telegram.org/api/folders#peer-folders)|
|ttl\_period|[int](/API_docs/types/int.html) | Optional|Time To Live of all messages in this chat; once a message is this many seconds old, it must be deleted.|
|theme\_emoticon|[string](/API_docs/types/string.html) | Optional|Emoji associated with chat theme|
|private\_forward\_name|[string](/API_docs/types/string.html) | Optional|Anonymized text to be shown instead of the user's name on forwarded messages|
|bot\_group\_admin\_rights|[ChatAdminRights](/API_docs/types/ChatAdminRights.html) | Optional|A [suggested set of administrator rights](https://core.telegram.org/api/rights#suggested-bot-rights) for the bot, to be shown when adding the bot as admin to a group, see [here for more info on how to handle them »](https://core.telegram.org/api/rights#suggested-bot-rights).|
|bot\_broadcast\_admin\_rights|[ChatAdminRights](/API_docs/types/ChatAdminRights.html) | Optional|A [suggested set of administrator rights](https://core.telegram.org/api/rights#suggested-bot-rights) for the bot, to be shown when adding the bot as admin to a channel, see [here for more info on how to handle them »](https://core.telegram.org/api/rights#suggested-bot-rights).|
|premium\_gifts|Array of [PremiumGiftOption](/API_docs/types/PremiumGiftOption.html) | Optional|Telegram Premium subscriptions gift options|
|wallpaper|[WallPaper](/API_docs/types/WallPaper.html) | Optional|[Wallpaper](https://core.telegram.org/api/wallpapers) to use in the private chat with the user.|
|stories|[PeerStories](/API_docs/types/PeerStories.html) | Optional|



### Type: [UserFull](/API_docs/types/UserFull.html)


### Example:

```
$userFull = ['_' => 'userFull', 'blocked' => Bool, 'phone_calls_available' => Bool, 'phone_calls_private' => Bool, 'can_pin_message' => Bool, 'has_scheduled' => Bool, 'video_calls_available' => Bool, 'voice_messages_forbidden' => Bool, 'translations_disabled' => Bool, 'stories_pinned_available' => Bool, 'blocked_my_stories_from' => Bool, 'wallpaper_overridden' => Bool, 'contact_require_premium' => Bool, 'read_dates_private' => Bool, 'id' => long, 'about' => 'string', 'settings' => PeerSettings, 'personal_photo' => Photo, 'profile_photo' => Photo, 'fallback_photo' => Photo, 'notify_settings' => PeerNotifySettings, 'bot_info' => BotInfo, 'pinned_msg_id' => int, 'common_chats_count' => int, 'folder_id' => int, 'ttl_period' => int, 'theme_emoticon' => 'string', 'private_forward_name' => 'string', 'bot_group_admin_rights' => ChatAdminRights, 'bot_broadcast_admin_rights' => ChatAdminRights, 'premium_gifts' => [PremiumGiftOption, PremiumGiftOption], 'wallpaper' => WallPaper, 'stories' => PeerStories];
```  
