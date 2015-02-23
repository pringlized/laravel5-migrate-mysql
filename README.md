# laravel5-migrate-mysql
A Laravel 5 console command to create migration files from a MYSQL database.  It will create individual files with a timestamp.

This command was built upon from the prior work of @Christopher Pitt, @michaeljcalkins and @Lee Zhen Yong.  Thanks guys!

To get it working:
- Copy MigrateMysqlSchemaCommand.php to app\Console\Commands
- Add 'App\Console\Commands\MigrateMysqlSchemaCommand' to $commands in app\Console\Kernel.php
