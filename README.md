# celeryTest

Setup celery periodic task with django. Refer to tutorial from [here](https://medium.com/@ksarthak4ever/django-handling-periodic-tasks-with-celery-daaa2a146f14)

To install required packages:
```
pip install -r requirements.txt
```

Need to setup a local redis server.

Command to start celery and celery beat:
```
celery -A celeryTest worker -l info -B --scheduler django_celery_beat.schedulers:DatabaseScheduler
```
