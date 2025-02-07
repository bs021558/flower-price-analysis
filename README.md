## 화훼가격과 거시지표를 이용한 데이터 분석
ETL 프로세스를 통해 데이터웨어하우스에 데이터를 적재하고 대시보드 구성해 보는 프로젝트
## 🌻목표
 - 화훼 데이터를 활용하여 __`일자별 화훼 가격 대시보드`__ 를 생성하는 것을 목표로 합니다.
 - 데이터 수집, 전처리, GCS에 저장 및 Bigquery 적재를 자동화 하는 __End-to-end 파이프라인을 경험__ 합니다.
 - 데이터웨어하우스에 적재된 데이터를 이용하여 __대시보드를 생성__ 합니다.
------------
## 🌼사용 데이터
- [일자별 화훼 경매 정보](https://flower.at.or.kr/api/apiOpenInfo.do)
- [기상청 데이터](https://data.kma.go.kr/data/grnd/selectAsosRltmList.do?pgmNo=36&tabNo=2)
- [학사일정](https://open.neis.go.kr/portal/data/service/selectServicePage.do?page=1&rows=10&sortColumn=&sortDirection=&infId=OPEN17220190722175038389180&infSeq=2)
## 🌼프로젝트 구조
![Untitled-2024-01-13-0010 excalidraw](https://github.com/es3442/ETL_Airflow_Flower/assets/77157003/7ddc9160-e4d9-49e1-8b72-7a76dbc02976)
1. API 호출을 통한 __데이터 수집 및 데이터 전처리__
2. __클라우드 스토리지에 데이터 저장__ (Google Cloud Storage)
3. Google cloud storage에 저장된 파일을 __데이터 웨어하우스에 적재__ (Bigquery)
4. 데이터 웨어하우스(Bigquery) 대시보드(Superset)에 연결
5. __대시보드 생성 및 데이터 분석__ 
