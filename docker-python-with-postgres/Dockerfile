FROM python:3.8-alpine

LABEL author="saoj07@gmail.com"

COPY script.py /app/script.py
COPY requirements.txt /app/requirements.txt

WORKDIR /app

RUN apk update && apk add postgresql-dev gcc python3-dev musl-dev

RUN pip install -r requirements.txt

CMD [ "python", "./script.py" ]