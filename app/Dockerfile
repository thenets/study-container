FROM alpine

RUN set -x \
    && apk add python3 py3-pip \
    && pip install flask

ENV FLASK_ENV=development
ENV FLASK_APP=/app/main.py

WORKDIR /app

ADD ./src/ /app

CMD ["flask", "run", "--host=0.0.0.0"]
