FROM python:3.7-alpine

RUN pip install --upgrade pip
RUN pip install django
RUN mkdir /app
WORKDIR /app
RUN django-admin.py startproject MyProject
WORKDIR /app/MyProject
RUN python manage.py migrate

EXPOSE 8000/tcp
EXPOSE 8001/tcp
EXPOSE 8002/tcp
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
