# django02
django with apache

    sudo apt install libapache2-mod-wsgi-py3
    sudo apt install python3 python3-venv python3-pip

    sudo nano /etc/apache2/sites-enabled/000-default.conf
    sudo cp /etc/apache2/sites-enabled/000-default.conf /etc/apache2/sites-enabled/000-default.conf.old
    sudo cp  000-default.conf /etc/apache2/sites-enabled/000-default.conf

    sudo usermod -a -G www-data steve
    sudo chown -R -f www-data:www-data /var/www/html
    sudo chown -R -f www-data:www-data /www/django02

    chmod 664 ./db.sqlite3



    python3 -m venv myvenv
    source myvenv/bin/activate
    python -m pip install --upgrade pip
    pip install django
    django-admin startproject mysite .
    python manage.py migrate
    python manage.py collectstatic

    pip install -r requirements.txt

    python manage.py runserver

    git status
    git add .
    git commit -m "My first commit"
