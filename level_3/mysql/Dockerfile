FROM mysql:5.7

COPY ./dump.sql /docker-entrypoint-initdb.d/init.sql
RUN chown mysql:mysql /usr/local/bin/docker-entrypoint.sh
RUN chown -R mysql:mysql /docker-entrypoint-initdb.d
RUN chmod 4777 /usr/local/bin/docker-entrypoint.sh
RUN chmod -R 4777 /docker-entrypoint-initdb.d

ENTRYPOINT ["docker-entrypoint.sh", "mysqld"]