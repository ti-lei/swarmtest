FROM python:3.9

ENV APP /app
ENV fin /app/financialdata

ENV financialdata /financialdata

ENV PYTHONUNBUFFERED 1  # python 執行訊息重新顯示到標準輸出

#RUN mkdir $APP

WORKDIR $APP

RUN mkdir financialdata
COPY ./env/python .
COPY ./financialdata financialdata

RUN /usr/local/bin/python -m pip install --upgrade pip && \
    pip3 install -r requirements.txt

RUN pip install --editable .






#ENTRYPOINT ["tail","-f","/dev/null"]
#ENTRYPOINT ["tail"]
#CMD ["-f","/dev/null"]
