---
title: "Database"
description: "MadelineProto optionally can keep some of its internal data in a database, such as mysql, mariadb, postgres or redis (you can also add your own!), reducing RAM usage.   "
nav_order: 14
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Database

MadelineProto *optionally* can keep some of its internal data in a database, such as mysql, mariadb, postgres or redis (you can also [add your own](https://github.com/danog/MadelineProto/tree/v8/src/Db)!), reducing RAM usage.   

On first start after switching type all data will be migrated from the previous backend to the new one. 
Database to memory migration is also supported.

Databases and tables will be created automatically.  

You can also directly connect the [event handler](/docs/UPDATES.html#built-in-database-driver) using the same async MySQL/Postgres/Redis ORM used by MadelineProto internally.  

Related settings:  

* [\danog\MadelineProto\Settings\Database\Memory: Memory backend settings.](../PHP/danog/MadelineProto/Settings/Database/Memory.html)
* [\danog\MadelineProto\Settings\Database\Mysql: MySQL backend settings.](../PHP/danog/MadelineProto/Settings/Database/Mysql.html) MariaDb 10.2+ or Mysql 5.6+ required.
* [\danog\MadelineProto\Settings\Database\Postgres: Postgres backend settings.](../PHP/danog/MadelineProto/Settings/Database/Postgres.html)
* [\danog\MadelineProto\Settings\Database\Redis: Redis backend settings.](../PHP/danog/MadelineProto/Settings/Database/Redis.html)

See [the settings documentation for more info](SETTINGS.html).  

### Mysql example (low memory usage):

```php
$settings = (new \danog\MadelineProto\Settings\Database\Mysql)
    ->setUri('tcp://localhost')
    ->setPassword('pass');

$API = new \danog\MadelineProto\API('session.madeline', $settings);
```

**WARNING**: Make sure to run `SET GLOBAL max_connections = 100000;` as root in the mysql/mariadb console, **regardless of the limit you set in the settings**.  
Make sure to run the command **after every system restart**, or modify the database configuration file to set the maximum connection limit to `100000`.  

### Postgres example (low memory usage):

```php
$settings = (new \danog\MadelineProto\Settings\Database\Postgres)
    ->setUri('tcp://localhost')
    ->setPassword('pass');
```

### Redis example (medium memory usage, faster access):

```php
$settings = (new \danog\MadelineProto\Settings\Database\Redis)
    ->setUri('redis://127.0.0.1')
    ->setPassword('pass');
```

### Memory example (medium-high memory usage, fastest access):

```php
$settings = new \danog\MadelineProto\Settings\Database\Memory;
```

<a href="https://docs.madelineproto.xyz/docs/SETTINGS.html">Next section</a>