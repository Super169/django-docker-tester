# django-docker-tester
Testing project for dockerized django project


| v1.0 | Build empty project in docker build                  |
| v1.1 | copy from existing empty project                     |
| v1.2 | Update db.sqlite3 with pre-set superuser for testing |

Windows command to use local db.sqlite3 in E:\Data:

  docker run --rm -d -p 8000:8000 -v e:\\data\\db.sqlite3:/app/MyProject/db.sqlite3 super169/django-docker-tester

Enjoy!