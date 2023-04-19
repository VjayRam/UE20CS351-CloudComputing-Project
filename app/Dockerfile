FROM python:3-alpine
RUN mkdir /flask_app
WORKDIR /flask_app
COPY requirements.txt /flask_app
RUN pip install --upgrade pip
RUN pip install -r /flask_app/requirements.txt
COPY . /flask_app
EXPOSE 5000
CMD [ "python", "app.py" ]