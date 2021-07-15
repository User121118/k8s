FROM krdsite24/djangob
ENV APP_HOME /usr/src/app
WORKDIR /usr/src/app
COPY ./ $APP_HOME
#RUN apt-get update
#RUN pip3 install --upgrade pip
#RUN chmod 777 -R $APP_HOME && chmod 777 -R /usr/local
#RUN ulimit -n 1000 && pip install --default-timeout=200 -r $APP_HOME/requirements.txt
#RUN pip install gunicorn==19.9.0 && pip install gunicorn[gthread]
EXPOSE 8000
#CMD ["gunicorn", "--bind", ":8000",  "smartstores.wsgi"]
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]