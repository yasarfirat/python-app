FROM alpine:3.7

RUN mkdir -p /app
WORKDIR /app
COPY . /app

RUN apk add --update \
    python \
    py-pip \
    py-mysqldb 

RUN pip install MySQL-python
RUN pip install Flask

ENV MYSQL_USERNAME=
ENV MYSQL_PASSWORD=	 
ENV MYSQL_DB=
ENV MYSQL_HOST=
ENV MYSQL_PORT=

EXPOSE 3000

CMD [ "python","application.py"]