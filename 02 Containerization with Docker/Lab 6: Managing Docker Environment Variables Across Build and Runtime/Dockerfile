FROM python:3.15.0a8-alpine3.23

WORKDIR /app

RUN pip install flask

ENV APP_MODE=production
ENV APP_REGION=canada-west

COPY ./Docker-3 .

USER daemon
EXPOSE 8080

CMD [ "python", "app.py" ]