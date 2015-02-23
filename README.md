# Laravel 5 Mysql Migration Command
A Laravel 5 console command to create migration files from a MYSQL database.  It will create individual files with a timestamp.

This command was built upon from the prior work of @Christopher Pitt, @michaeljcalkins and @Lee Zhen Yong.  Thanks guys!

## Installation
1. Copy MigrateMysqlSchemaCommand.php to app\Console\Commands
2. Add 'App\Console\Commands\MigrateMysqlSchemaCommand' to $commands in app\Console\Kernel.php

## Usage
This is a first version for Laravel 5.  dbName is required while --ignore and --only are optional. You can't use only & ignore together.  Choose one, the other, or neither. Running the command will give you line item feedback of the migration files it creates. Once installed you run any of the following 3 scenarios. 

**The entire database**

```php artisan migrate:schema-mysql dbName```

**Ignoring tables**

You can ignore tables by using the following command. NOTE: The 'migrations' table will always ignored whether you use the --ignore arguement or not.
```
php artisan migrate:schema-mysql dbName --ignore=table1,table2
```

**Only specific tables**

To only create migrations from specific tables use --only.
```
php artisan migrate:schema-mysql dbName --only=table1,table2
```

## Credit
Thanks to "bruceoutdoors" [original class](https://gist.github.com/bruceoutdoors/9166186) and "adamkearsley" [for a readme template] (https://github.com/adamkearsley/laravel-convert-migrations)
