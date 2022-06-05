FROM python:3.9

ENV APP /app

ENV PYTHONUNBUFFERED 1  # python 執行訊息重新顯示到標準輸出

#RUN mkdir $APP

WORKDIR $APP

#RUN mkdir financialdata

# env 裡面有包含python要安裝的套件 都放到app的目錄裡
COPY ./env/python .

# 把 Project 資料夾裡的東西(整個financialdata module 和 api服務 都放到 app/Project資料夾)
COPY ./Project Project


RUN /usr/local/bin/python -m pip install --upgrade pip && \
    pip3 install -r requirements.txt

WORKDIR Project
RUN pip install --editable .

#ENV PYTHONPATH "${PYTHONPATH}:/app/financialdata/financialdata"