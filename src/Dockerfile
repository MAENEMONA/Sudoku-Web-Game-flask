FROM python:3.10.0

WORKDIR /app

COPY . /app

RUN pip install -r requirements.txt

EXPOSE 5000

RUN pip install gunicorn

CMD [ "python3", "-m", "gunicorn", "--bind", "0.0.0.0:5000", "wsgi:app"]
