FROM python:latest

EXPOSE 80

ADD . /app

WORKDIR /app

RUN pip install uwsgi
RUN pip install -r requirements.txt

CMD [ "uwsgi", "--socket", "0.0.0.0:3031", \
               "--uid", "uwsgi", \
               "--plugins", "python3", \
               "--protocol", "uwsgi", \
               "--wsgi", "main:application" ]