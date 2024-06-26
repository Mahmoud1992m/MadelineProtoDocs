---
title: "danog\\MadelineProto\\RPCErrorException: Indicates an error returned by Telegram's API."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\RPCErrorException`
[Back to index](../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Indicates an error returned by Telegram's API.  



## Properties
* `$rpc`: `string` RPC error
* `$tlTrace`: `string` TL trace.

## Method list:
* [`localizeMessage(mixed $method, int $code, string $error): string`](#localizeMessage)
* [`getLocalization(): string`](#getLocalization)
* [`setLocalization(string $localization): void`](#setLocalization)
* [`__construct(string $rpc, int $code = 0, mixed $caller = '', ?\danog\MadelineProto\Exception $previous = NULL)`](#__construct)
* [`getMessage(): string`](#getMessage)
* [`getCode()`](#getCode)
* [`getFile(): string`](#getFile)
* [`getLine(): int`](#getLine)
* [`getTrace(): array`](#getTrace)
* [`getPrevious(): ?Throwable`](#getPrevious)
* [`getTraceAsString(): string`](#getTraceAsString)
* [`updateTLTrace(array $trace): void`](#updateTLTrace)
* [`getTLTrace(): string`](#getTLTrace)
* [`setTLTrace(string $tlTrace): void`](#setTLTrace)
* [`prettifyTL(string $init = '', array $trace = NULL): void`](#prettifyTL)

## Methods:
### <a name="localizeMessage"></a> `localizeMessage(mixed $method, int $code, string $error): string`




Parameters:

* `$method`: `mixed`   
* `$code`: `int`   
* `$error`: `string`   



### <a name="getLocalization"></a> `getLocalization(): string`

Get localized error name.



### <a name="setLocalization"></a> `setLocalization(string $localization): void`

Set localized error name.


Parameters:

* `$localization`: `string`   



### <a name="__construct"></a> `__construct(string $rpc, int $code = 0, mixed $caller = '', ?\danog\MadelineProto\Exception $previous = NULL)`




Parameters:

* `$rpc`: `string`   
* `$code`: `int`   
* `$caller`: `mixed`   
* `$previous`: `?\danog\MadelineProto\Exception`   


#### See also: 
* [`\danog\MadelineProto\Exception`: Basic exception.](../../danog/MadelineProto/Exception.html)




### <a name="getMessage"></a> `getMessage(): string`





### <a name="getCode"></a> `getCode()`





### <a name="getFile"></a> `getFile(): string`





### <a name="getLine"></a> `getLine(): int`





### <a name="getTrace"></a> `getTrace(): array`





### <a name="getPrevious"></a> `getPrevious(): ?Throwable`




#### See also: 
* `Throwable`




### <a name="getTraceAsString"></a> `getTraceAsString(): string`





### <a name="updateTLTrace"></a> `updateTLTrace(array $trace): void`

Update TL trace.


Parameters:

* `$trace`: `array`   



### <a name="getTLTrace"></a> `getTLTrace(): string`

Get TL trace.



### <a name="setTLTrace"></a> `setTLTrace(string $tlTrace): void`

Set TL trace.


Parameters:

* `$tlTrace`: `string` TL trace  



### <a name="prettifyTL"></a> `prettifyTL(string $init = '', array $trace = NULL): void`

Generate async trace.


Parameters:

* `$init`: `string` Method name  
* `$trace`: `array` Async trace  



---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
