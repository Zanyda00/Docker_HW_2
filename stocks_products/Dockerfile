FROM python:3.11
COPY . /srs 
WORKDIR srs
RUN pip install -r requirements.txt --no-cache
RUN python3 manage.py migrate
EXPOSE 8000
CMD python3 manage.py runserver 0.0.0.0:8000