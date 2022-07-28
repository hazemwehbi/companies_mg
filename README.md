### DESCRIPTION ###

project to manage companies and their employees.

Basic Laravel Auth: ability to log in as administrator
Use database seeds to create first user with email admin@admin.com and password “password”
CRUD functionality (Create / Read / Update / Delete) for two menu items: Companies and Employees.
Companies DB table consists of these fields: Name (required), email, logo (minimum 100×100), website
Employees DB table consists of these fields: First name (required), last name (required), Company (foreign key to Companies), email, phone
Use database migrations to create those schemas above
Use database seeds to create at least 10 initial companies
Store companies logos in storage/app/public folder and make them accessible from public
Use basic Laravel resource controllers with default methods – index, create, store etc.
Use Laravel’s validation function, using Request classes
Use Laravel’s pagination for showing Companies/Employees list, 10 entries per page
Create authentication without using Laravel fortify.
Email notification: send email whenever new company is entered (use Mailgun or Mailtrap)
Testing with phpunit

### PRESEREQUISITES ###

- php8.1
- composer

### CI/CD Github (.github/workflows/php.yml)
You can find the CI/CD Github pipeline for deployment and production process

### UNIT TEST ###

- php artisan test --env=testing

### Execute Process ###
- `php artisan key:generate`
- `php artisan migrate --seed`

### PORT ###

<<<<<<< HEAD
- localhost:80

### Docker
Test MySQL server
- Give Docker permission, `sudo chmod 666 /var/run/docker.sock`
- Create MySQL image: `docker build -t testdb .`
- Run MySQL: `docker run --detach --name=testdb --publish 3306:3306 testdb -e MYSQL_ROOT_PASSWORD=admin`
=======
- localhost:8000
>>>>>>> bd4c4bc020037196e822c17bb9ca00973d551331
