FROM python:3.10.8

ENV MAIN_DIR /usr/src/app

WORKDIR $MAIN_DIR

COPY . $MAIN_DIR

RUN pip install pipenv

RUN pipenv requirements > requirements.txt

RUN pip install -r requirements.txt

RUN pip install -e .

CMD ["bot_assist"]