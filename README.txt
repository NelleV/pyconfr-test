
- `pip install -r requirements.txt`
- `python manage.py syncdb`
- `python manage.py loaddata fixtures/*`

./bin/django loaddata src/pyconfr/fixtures/*.json
./bin/django collectstatic
./bin/django compilemessages
Start it in dev mode:

./bin/django runserver
Gunicorn start for prod:

./bin/django run_gunicorn -b 127.0.0.1:8001
