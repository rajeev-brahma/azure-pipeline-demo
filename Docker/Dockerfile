FROM python:3.11.7-alpine
 
WORKDIR /usr/src/app
 
ENV PYTHONDONTWRITEBYTECODE 1
 
ENV PYTHONRUNBUFFERED 1
 
RUN pip install --upgrade pip
 
COPY ./requirements.txt /usr/src/app/requirements.txt
 
RUN pip install -r requirements.txt
 
COPY ./demo_project /usr/src/app/
 
EXPOSE 8000
 
CMD ["python","manage.py","runserver","0.0.0.0:8000"]


