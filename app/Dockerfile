FROM python:latest

COPY requirements.txt /tmp/
RUN pip install --requirement /tmp/requirements.txt

WORKDIR /src/

CMD [ "python", "app.py"]