---
title: "danog\\MadelineProto\\Exception: Basic exception."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\Exception`
[Back to index](../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Basic exception.  



## Properties
* `$tlTrace`: `string` TL trace.

## Method list:
* [`__construct(mixed $message = NULL, mixed $code = 0, ?Throwable $previous = NULL, mixed $file = NULL, mixed $line = NULL)`](#__construct)
* [`extension(string $extensionName): self`](#extension)
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
### <a name="__construct"></a> `__construct(mixed $message = NULL, mixed $code = 0, ?Throwable $previous = NULL, mixed $file = NULL, mixed $line = NULL)`




Parameters:

* `$message`: `mixed`   
* `$code`: `mixed`   
* `$previous`: `?Throwable`   
* `$file`: `mixed`   
* `$line`: `mixed`   


#### See also: 
* `Throwable`




### <a name="extension"></a> `extension(string $extensionName): self`

Complain about missing extensions.


Parameters:

* `$extensionName`: `string` Extension name  



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
