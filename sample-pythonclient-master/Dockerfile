FROM python:3
WORKDIR /usr/src/app
COPY . .
RUN pip3 install -r requirements.txt
RUN pip install gunicorn
CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 app:app
