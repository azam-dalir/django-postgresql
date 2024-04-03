one-part of django-project

part1 >>>>> First clone the project-----Clone using the web URL. github-account > repository > code > copy URL > project folder > address bar > cmd > git clone (paste URL address)

part2 >>>>> make sure Docker is running.

If you are on windows click on the Docker Desktop icon and wait for about a minute.

part3 >>>>> run this command:

docker-compose up --build It will create two containers: One for Django and one for PostgreSql as the database for the project. All the required packages will be installed.

part 4 >>>>> Install a new package. Attention: If you want to install a package for django project you should run this command:

docker-compose exec web pip install

part5 >>>>> Don't forget to add the new package to requirements.txt for further use:

docker-compose exec web pip freeze > requirements.txt

for insert your project in new repository you should run this comment: project-folder > address bar > cmd > git init
git status
git add .
git commit -m "initial commit"

git remote add origin https://github.com/azam-dalir/django-postgresql.git
git branch -M main
git push -u origin main
