FROM python:3.11.5-bookworm

WORKDIR /usr/src/app

RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install -r requirements.txt
COPY . /usr/src/app

EXPOSE 8000
CMD ["/bin/sh", "-c", "python3 manage.py runserver"]