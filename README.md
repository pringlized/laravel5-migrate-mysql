# laravel5-migrate-mysql
A Laravel 5 console command to create migration files from a MYSQL database.  It will create individual files with a timestamp.

This command was built upon from the prior work of @Christopher Pitt, @michaeljcalkins and @Lee Zhen Yong.  Thanks guys!

## Installation
1. Copy MigrateMysqlSchemaCommand.php to app\Console\Commands
2. Add 'App\Console\Commands\MigrateMysqlSchemaCommand' to $commands in app\Console\Kernel.php

## Usage
This is a first version for Laravel 5.  Once installed you run it by using artisan:  `php artisan migrate:schema-mysql --db=name --ignore=table1,table2`.  --db is required while --ignore is optional.  It will give you line item feedback of the migration files it creates.

## Credit
Thanks to "bruceoutdoors" [original class](https://gist.github.com/bruceoutdoors/9166186).
