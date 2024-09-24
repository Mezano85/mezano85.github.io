FROM jupyter/base-notebook

ENV DATA_HOME /usr/src/data
WORKDIR /$DATA_HOME

ADD .env ./
ADD requirements.txt ./
RUN pip install -r requirements.txt