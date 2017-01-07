# Vagrant-Django
Vagrant + Django (No known issues)

This machine contains: MySQL, Apache, PHP, Python, Django and Nodejs.

How to setup:

    git clone https://github.com/Externoak/Vagrant-Django-CMS.git
    
    cd Vagrant-Django-CMS

    vagrant up


#### Once vagrant has finish everything should be working perfectly.

This machine will automatically have a working server on IP assigned to the machine on port :8000



# Start your own project in Django.

If you want to create your own project follow these steps:

    vagrant ssh

    cd django_cms

W/O Quotes.

    django-admin.py startproject “Name of your Project”

    cd “Name of your Project”
    
    sudo python manage.py runserver “IP:PORT”

Allowhost error:
    If your'e getting Allowhost error you must modify the following.
          
           sudo nano “Name of your Project”/settings.py
                Modify ALLOWED_HOSTS = ['"Your IP"']
