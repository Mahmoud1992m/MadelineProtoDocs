---
title: "danog\\MadelineProto\\StrTools: Some tools."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\StrTools`
[Back to index](../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Some tools.  




## Constants
* `danog\MadelineProto\StrTools::ALL_MIMES`: 


## Method list:
* [`mbStrlen(string $text): int`](#mbstrlen-string-text-int)
* [`mbSubstr(string $text, int $offset, null|int $length = NULL): string`](#mbsubstr-string-text-int-offset-null-int-length-null-string)
* [`mbStrSplit(string $text, int $length): string[]`](#mbstrsplit-string-text-int-length-string)
* [`htmlToMessageEntities(string $html): \danog\MadelineProto\TL\Conversion\DOMEntities Object containing message and entities`](#htmltomessageentities-string-html-danog-madelineproto-tl-conversion-domentities-object-containing-message-and-entities)
* [`markdownToMessageEntities(string $markdown): \danog\MadelineProto\TL\Conversion\MarkdownEntities Object containing message and entities`](#markdowntomessageentities-string-markdown-danog-madelineproto-tl-conversion-markdownentities-object-containing-message-and-entities)
* [`entitiesToHtml(string $message, list<\danog\MadelineProto\EventHandler\Message\Entities\MessageEntity|array{_: string, offset: int, length: int}> $entities, bool $allowTelegramTags = false): string`](#entitiestohtml-string-message-list-danog-madelineproto-eventhandler-message-entities-messageentity-array-_-string-offset-int-length-int-entities-bool-allowtelegramtags-false-string)
* [`toCamelCase(string $input): string`](#tocamelcase-string-input-string)
* [`toSnakeCase(string $input): string`](#tosnakecase-string-input-string)
* [`htmlEscape(string $what): string`](#htmlescape-string-what-string)
* [`markdownEscape(string $what): string`](#markdownescape-string-what-string)
* [`markdownCodeblockEscape(string $what): string`](#markdowncodeblockescape-string-what-string)
* [`markdownCodeEscape(string $what): string`](#markdowncodeescape-string-what-string)
* [`markdownUrlEscape(string $what): string`](#markdownurlescape-string-what-string)
* [`getMimeFromExtension(string $extension, string $default): string`](#getmimefromextension-string-extension-string-default-string)
* [`getExtensionFromMime(string $mime): string`](#getextensionfrommime-string-mime-string)
* [`getExtensionFromLocation(mixed $location, string $default): string`](#getextensionfromlocation-mixed-location-string-default-string)
* [`getMimeFromFile(string $file): string`](#getmimefromfile-string-file-string)
* [`getMimeFromBuffer(string $buffer): string`](#getmimefrombuffer-string-buffer-string)

## Methods:
### `mbStrlen(string $text): int`

Get Telegram UTF-8 length of string.


Parameters:

* `$text`: `string` Text  



### `mbSubstr(string $text, int $offset, null|int $length = NULL): string`

Telegram UTF-8 multibyte substring.


Parameters:

* `$text`: `string` Text to substring  
* `$offset`: `int` Offset  
* `$length`: `null|int` Length  



### `mbStrSplit(string $text, int $length): string[]`

Telegram UTF-8 multibyte split.


Parameters:

* `$text`: `string` Text  
* `$length`: `int` Length  



### `htmlToMessageEntities(string $html): \danog\MadelineProto\TL\Conversion\DOMEntities Object containing message and entities`

Manually convert HTML to a message and a set of entities.
NOTE: You don't have to use this method to send HTML messages.  
  
This method is already called automatically by using parse_mode: "HTML" in messages.sendMessage, messages.sendMedia, et cetera...

Parameters:

* `$html`: `string`   


Return value: Object containing message and entities

#### See also: 
* [https://docs.madelineproto.xyz/API_docs/methods/messages.sendMessage.html#usage-of-parse_mode](https://docs.madelineproto.xyz/API_docs/methods/messages.sendMessage.html#usage-of-parse_mode)




### `markdownToMessageEntities(string $markdown): \danog\MadelineProto\TL\Conversion\MarkdownEntities Object containing message and entities`

Manually convert markdown to a message and a set of entities.
NOTE: You don't have to use this method to send Markdown messages.  
  
This method is already called automatically by using parse_mode: "Markdown" in messages.sendMessage, messages.sendMedia, et cetera...

Parameters:

* `$markdown`: `string`   


Return value: Object containing message and entities

#### See also: 
* [https://docs.madelineproto.xyz/API_docs/methods/messages.sendMessage.html#usage-of-parse_mode](https://docs.madelineproto.xyz/API_docs/methods/messages.sendMessage.html#usage-of-parse_mode)




### `entitiesToHtml(string $message, list<\danog\MadelineProto\EventHandler\Message\Entities\MessageEntity|array{_: string, offset: int, length: int}> $entities, bool $allowTelegramTags = false): string`

Convert a message and a set of entities to HTML.


Parameters:

* `$message`: `string`   
* `$entities`: `list<\danog\MadelineProto\EventHandler\Message\Entities\MessageEntity|array{_: string, offset: int, length: int}>`   
* `$allowTelegramTags`: `bool` Whether to allow telegram-specific tags like tg-spoiler, tg-emoji, mention links and so on...  


#### See also: 
* [`\danog\MadelineProto\EventHandler\Message\Entities\MessageEntity`: Master class for message entities.](../../danog/MadelineProto/EventHandler/Message/Entities/MessageEntity.html)




### `toCamelCase(string $input): string`

Convert to camelCase.


Parameters:

* `$input`: `string` String  



### `toSnakeCase(string $input): string`

Convert to snake_case.


Parameters:

* `$input`: `string` String  



### `htmlEscape(string $what): string`

Escape string for MadelineProto's HTML entity converter.


Parameters:

* `$what`: `string` String to escape  



### `markdownEscape(string $what): string`

Escape string for markdown.


Parameters:

* `$what`: `string` String to escape  



### `markdownCodeblockEscape(string $what): string`

Escape string for markdown codeblock.


Parameters:

* `$what`: `string` String to escape  



### `markdownCodeEscape(string $what): string`

Escape string for markdown code section.


Parameters:

* `$what`: `string` String to escape  



### `markdownUrlEscape(string $what): string`

Escape string for URL.


Parameters:

* `$what`: `string` String to escape  



### `getMimeFromExtension(string $extension, string $default): string`

Get mime type from file extension.


Parameters:

* `$extension`: `string` File extension  
* `$default`: `string` Default mime type  



### `getExtensionFromMime(string $mime): string`

Get extension from mime type.


Parameters:

* `$mime`: `string` MIME type  



### `getExtensionFromLocation(mixed $location, string $default): string`

Get extension from file location.


Parameters:

* `$location`: `mixed` File location  
* `$default`: `string` Default extension  



### `getMimeFromFile(string $file): string`

Get mime type of file.


Parameters:

* `$file`: `string` File  



### `getMimeFromBuffer(string $buffer): string`

Get mime type from buffer.


Parameters:

* `$buffer`: `string` Buffer  



---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
