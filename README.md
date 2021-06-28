# Chart to python api and postgres

Install Python API Charts

helm install releasename miltex/python-api-postgres --set DATABASE_URL=postgresql://milton:milton@localhost:5432/python-api

Variables should be setting:

FLASK_APP=run.py
FLASK_DEBUG=0
FLASK_ENV=production
TESTING=False
DEBUG=False
SQLALCHEMY_TRACK_MODIFICATIONS=True
DATABASE_URL=postgresql://admin:secret@localhost:5432/python-api
GUNICORN_WORKERS=1
LOG_LEVEL=debug
SK=yS6xsprA0gTuBWO_vV2JVQ
CSRF_ENABLED=True
BOOTSTRAP_FONTAWESOME = True
RESTPLUS_MASK_SWAGGER = False
#### In production, set to a higher number, like 31556926
SEND_FILE_MAX_AGE_DEFAULT=0

## Using API

http://ip:port/tasks/doc

http://ip:port/users/doc