FROM mysql:latest

COPY ./products.csv /products.csv
COPY ./users.csv /users.csv
COPY ./setup.sql /setup.sql
COPY ./seed.sql /seed.sql


ENTRYPOINT ["/entrypoint.sh"]
CMD ["mysqld", "--secure-file-priv=/", "--local-infile=ON"]
#CMD ["--secure-file-priv=/"]


