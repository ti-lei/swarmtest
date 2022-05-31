FROM mysql:8.0

RUN apt-get update

#RUN mkdir /FinMindProject

# 把專案目錄下的 docker-entrypoint-initdb.d 資料夾 copy 到 container裡面的 docker-entrypoint-initdb.d 資料夾內
COPY ./env/mysql/docker-entrypoint-initdb.d /docker-entrypoint-initdb.d/