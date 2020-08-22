
## Multi Authentication

This respository contains the files to create multi authentication.
The multi authentication can be acheived several ways in laravel. However , this module explains achieving using guard

## Steps
Using this admin and normal user can login

## Step 1

Create a project using laravel 7 and install laravel ui

composer require laravel/ui

php artisan ui bootstrap --auth

npm install && npm run dev

## Stemp 2

Create new table admins, model and controller using artisan command
Then do the changes as in the repo

php artisan make:model -m Admin
php artisan make:controller AdminController
php artisan make:controller Auth/AdminLoginController

create views for admin and login

## Step 3

Modify the config/auth to define guard
Modify the handle method of App\Http\Middleware\RedirectIfAuthenticated
Implement the unauthenticated function App\Exceptions\Handler

## Step 4

Create seeder for Admin creation to login as admin

