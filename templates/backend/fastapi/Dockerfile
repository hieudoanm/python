FROM python:3.13.1

ENV ENVIRONMENT='production'
ENV PORT='10000'

COPY main.py main.py
COPY Makefile Makefile
COPY requirements.txt requirements.txt

RUN python3 -m pip install -r requirements.txt
EXPOSE $PORT

ENTRYPOINT ["python3"]
CMD ["main.py"]
