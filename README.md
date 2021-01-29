The application uses Symfony 5.2.1. The pagination was done using KnpPaginatorBundle and it works every 5 records.

To run the project, please follow the instructions:
1. Change the MySQL credentials for the valid ones on the .env file
2. Run "composer install" to fetch the all needed vendors
3. Create the databases. Run "bin/console doctrine:database:create"
4. Make migrations. Run "bin/console doctrine:migrations:migrate -n -q"
5. Let's load fixtures. Run "bin/console doctrine:fixtures:load" (mark [yes])
6. Let's run the application by preferable method. In this case I use: php -S 127.0.0.1:8000 -t public

By now we have one existing user in database with the credentials of:
Login: lukas.stankus@hotmail.com
Password: miami100

Unity/funtional testing
1. Unit tests can easily be found under ./tests.
2. CSV exporter test. Run "./bin/phpunit tests/CsvServiceTest.php"
3. Login form test. Run "./bin/phpunit tests/UserLoginTest.php"
