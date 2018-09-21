FROM python:latest

EXPOSE 80

COPY requirements.txt /tmp/
RUN pip install --requirement /tmp/requirements.txt
COPY . /tmp/

WORKDIR /tmp/

# CMD [ "uwsgi", "" , "" ]