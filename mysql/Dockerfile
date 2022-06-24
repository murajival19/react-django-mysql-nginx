# mysql/Dockerfile
# set base image
FROM mysql:8.0.29

# set init
RUN echo "USE mysql;" > /docker-entrypoint-initdb.d/timezones.sql &&  mysql_tzinfo_to_sql /usr/share/zoneinfo >> /docker-entrypoint-initdb.d/timezones.sql

# set config data
COPY mysql/my.cnf /etc/mysql/conf.d/my.cnf
