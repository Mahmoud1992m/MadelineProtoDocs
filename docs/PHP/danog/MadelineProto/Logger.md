---
title: "danog\\MadelineProto\\Logger: Logger class."
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\Logger`
[Back to index](../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Logger class.  




## Constants
* `danog\MadelineProto\Logger::FOREGROUND`: 

* `danog\MadelineProto\Logger::BACKGROUND`: 

* `danog\MadelineProto\Logger::SET`: 

* `danog\MadelineProto\Logger::RESET`: 

* `danog\MadelineProto\Logger::ULTRA_VERBOSE`: Ultra verbose logging.

* `danog\MadelineProto\Logger::VERBOSE`: Verbose logging.

* `danog\MadelineProto\Logger::NOTICE`: Notice logging.

* `danog\MadelineProto\Logger::WARNING`: Warning logging.

* `danog\MadelineProto\Logger::ERROR`: Error logging.

* `danog\MadelineProto\Logger::FATAL_ERROR`: Log only fatal errors.

* `danog\MadelineProto\Logger::DEFAULT_LOGGER`: Default logger (syslog).

* `danog\MadelineProto\Logger::FILE_LOGGER`: File logger.

* `danog\MadelineProto\Logger::ECHO_LOGGER`: Echo logger.

* `danog\MadelineProto\Logger::CALLABLE_LOGGER`: Callable logger.

* `danog\MadelineProto\Logger::LEVEL_ULTRA_VERBOSE`: Ultra verbose level.

* `danog\MadelineProto\Logger::LEVEL_VERBOSE`: Verbose level.

* `danog\MadelineProto\Logger::LEVEL_NOTICE`: Notice level.

* `danog\MadelineProto\Logger::LEVEL_WARNING`: Warning level.

* `danog\MadelineProto\Logger::LEVEL_ERROR`: Error level.

* `danog\MadelineProto\Logger::LEVEL_FATAL`: Fatal error level.

* `danog\MadelineProto\Logger::LOGGER_DEFAULT`: Default logger (syslog).

* `danog\MadelineProto\Logger::LOGGER_ECHO`: Echo logger.

* `danog\MadelineProto\Logger::LOGGER_FILE`: File logger.

* `danog\MadelineProto\Logger::LOGGER_CALLABLE`: Callable logger.

## Properties
* `$default`: `?self` Default logger instance.

## Method list:
* [`constructorFromSettings(\danog\MadelineProto\Settings\Logger $settings): self`](#constructorFromSettings)
* [`__construct(\danog\MadelineProto\Settings\Logger $settings, string $prefix = '')`](#__construct)
* [`truncate(): void`](#truncate)
* [`log(mixed $param, int $level = \self::NOTICE): void`](#log)
* [`logger(mixed $param, int $level = \self::NOTICE, string $file = ''): void`](#logger)
* [`getPsrLogger(): \Psr\Log\LoggerInterface`](#getPsrLogger)

## Methods:
### <a name="constructorFromSettings"></a> `constructorFromSettings(\danog\MadelineProto\Settings\Logger $settings): self`

Construct global static logger from MadelineProto settings.


Parameters:

* `$settings`: `\danog\MadelineProto\Settings\Logger` Settings instance  


#### See also: 
* [`\danog\MadelineProto\Settings\Logger`: Logger settings.](../../danog/MadelineProto/Settings/Logger.html)




### <a name="__construct"></a> `__construct(\danog\MadelineProto\Settings\Logger $settings, string $prefix = '')`

Construct logger.


Parameters:

* `$settings`: `\danog\MadelineProto\Settings\Logger`   
* `$prefix`: `string`   


#### See also: 
* [`\danog\MadelineProto\Settings\Logger`: Logger settings.](../../danog/MadelineProto/Settings/Logger.html)




### <a name="truncate"></a> `truncate(): void`

Truncate logfile.



### <a name="log"></a> `log(mixed $param, int $level = \self::NOTICE): void`

Log a message.


Parameters:

* `$param`: `mixed` Message  
* `$level`: `int` Logging level  



### <a name="logger"></a> `logger(mixed $param, int $level = \self::NOTICE, string $file = ''): void`

Log a message.


Parameters:

* `$param`: `mixed` Message to log  
* `$level`: `int` Logging level  
* `$file`: `string` File that originated the message  



### <a name="getPsrLogger"></a> `getPsrLogger(): \Psr\Log\LoggerInterface`

Get PSR logger.


#### See also: 
* `\Psr\Log\LoggerInterface`




---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
