FROM python:latest

RUN pip install -r requirements.txt

COPY . /app
WORKDIR /app

EXPOSE 80

CMD ["python", "app.py"]

#RUN mkdir -p /opt/services/flaskapp/src
#VOLUME ["/opt/services/flaskapp/src"]
# We copy the requirements.txt file first to avoid cache invalidations
#COPY requirements.txt /opt/services/flaskapp/src/
#WORKDIR /opt/services/flaskapp/src
#RUN pip install -r requirements.txt
#COPY . /opt/services/flaskapp/src
#EXPOSE 5090
