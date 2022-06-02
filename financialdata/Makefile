# sent task
sent-task:
	pipenv run python financialdata/producer.py taiwan_stock_price 2021-04-01 2021-04-12

# 建立 dev 環境變數
gen-dev-env-variable:
	python genenv.py

# 建立 staging 環境變數
gen-staging-env-variable:
	VERSION=STAGING python genenv.py

# 建立 release 環境變數
gen-release-env-variable:
	VERSION=RELEASE python genenv.py
	