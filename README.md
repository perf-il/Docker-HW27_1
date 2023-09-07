# Docker-HW27_1

Dockerfile:

FROM python:3

WORKDIR /code

COPY ./requirments.txt .

RUN pip install -r requirments.txt

COPY . .

CMD ["python", "manage.py", "runserver"]
