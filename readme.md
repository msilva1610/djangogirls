mkdir djanogirls
cd djangogirls
python3 -m venv myvenv
source /myvenv/bin/activate
deatectivate

pip install django

pip freeze > requirements.txt
pip install -r requirements.txt


django-admin startproject mysite .

python manage.py migrate
python manage.py runserver

python manage.py startapp blog


python manage.py makemigrations blog

python manage.py migrate blog

python manage.py runserver
python manage.py createsuperuser