FROM python:3.10
WORKDIR /app
COPY *.py .
COPY payment.ini .
COPY requirements.txt .
RUN pip3 install -r requirements.txt
CMD ["/usr/local/bin/uwsgi", "--ini", "payment.ini"]