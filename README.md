# Python: Getting Started

A barebones Django app, which can easily be deployed to Heroku.

This application supports the [Getting Started with Python on Heroku](https://devcenter.heroku.com/articles/getting-started-with-python) article - check it out.

## Running Locally

Make sure you have Python 3.7 [installed locally](http://install.python-guide.org). To push to Heroku, you'll need to install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli), as well as [Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

```sh
$ git clone https://github.com/heroku/python-getting-started.git
$ cd python-getting-started

# $ python3 -m venv getting-started
python -m venv getting-started
# $ pip install -r requirements.txt
pip install -r requirements.txt

# $ createdb python_getting_started
createdb python_getting_started

$ python manage.py migrate
$ python manage.py collectstatic

$ heroku local
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```sh
$ heroku create
$ git push heroku master

$ heroku run python manage.py migrate
$ heroku open
```
or

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Documentation

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)






<!-- …or create a new repository on the command line -->
echo "# python-django-sqlite3-heroku" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/jav2074/python-django-sqlite3-heroku.git
git push -u origin master
                
<!-- …or push an existing repository from the command line -->
git remote add origin https://github.com/jav2074/python-django-sqlite3-heroku.git
git push -u origin master



git remote set-url origin https://github.com/jav2074/python-django-sqlite3-heroku.git

<!-- Enumerar tus remotos existentes a fin de obtener el nombre de los remotos que deseas cambiar. -->
$ git remote -v
> origin  git@github.com:USERNAME/REPOSITORY.git (fetch)
> origin  git@github.com:USERNAME/REPOSITORY.git (push)
<!-- Cambiar tu URL remota de SSH a HTTPS con el comando git remote set-url. -->
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
<!-- Verificar que la URL remota ha cambiado. -->
$ git remote -v
<!-- # Verify new remote URL -->
> origin  https://github.com/USERNAME/REPOSITORY.git (fetch)
> origin  https://github.com/USERNAME/REPOSITORY.git (push)