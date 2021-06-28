# Q-Doctor - Docker/ Set Up
This is a simple laravel 8 CRUD app.
The repository is the code to one of my article on **Dev.to**, [Laravel 8 CRUD App, A simple guide](https://dev.to/kingsconsult/laravel-8-crud-bi9) the article will teach you how to create a CRUD app on Laravel 8, the method is applicable to Laravel 6 and also Laravel 7 
## CI CD via Circle CI
1. Pull repo from Git: https://github.com/Glendoni/qdoctor_docker.git
2. Create an CircleCI account: https://circleci.com/
3. Follow instructions to connect Circle CI to set up link to GitHub

## How to install and run on your local system
1. git clone https://github.com/Glendoni/q-doctor.git
2. Terminal cd [to root folder]/
3. Terminal run: docker-compose - build to pull down all dependencies  
4. Termiinal run: docker-compose up -d
5. Terminal run: docker exec -it  qdoctor_php-fpm_1  bash
6. In Docker Shell Run: cd source
7. In Docker Shell Run: composer update
8. If .env does not exsit in open docker shell: Run: cp .env.example .env
9. In Source folder open .env file and update the DB creds that can be found in the docker-compose.yml file  
10. Return back to the docker shell Run: php artisan key:generate
11. In Docker Shell Run: php artisan migrate
12. Visit page: http://localhost:10000/projects





![localhost](https://res.cloudinary.com/kingsconsult/image/upload/v1600705305/laravel%208%20modal/4_pp7r76.png)
10. Navigate to http://127.0.0.1:8000/projects
![CRUD](https://res.cloudinary.com/kingsconsult/image/upload/v1602364575/crud_llekuf.png)

## Operations
1. Create a project
2. View a project
3. Edit a project
4. Delete a project
5. View all projects
