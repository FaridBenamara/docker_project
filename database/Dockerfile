# Custom PostgreSQL Dockerfile
FROM postgres:latest

COPY ./init-scripts /docker-entrypoint-initdb.d/

ENV POSTGRES_DB=root
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=farid

EXPOSE 5432
