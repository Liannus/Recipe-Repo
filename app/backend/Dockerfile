FROM python:3.7

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir /backend_container
WORKDIR /backend_container

COPY requirements.txt /backend_container/
RUN pip install -r requirements.txt

COPY . .

EXPOSE 5000

