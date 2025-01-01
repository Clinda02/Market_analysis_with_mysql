# MySQL 고객 및 제품 데이터 분석

## 1. 프로젝트 개요 
<img src="https://github.com/user-attachments/assets/e7c4bcfc-4c35-4ff4-af33-e3bc9d4cb49f" width="600" height="400"/>

[MySQL의 ClassicModels 샘플 데이터베이스](https://www.mysqltutorial.org/getting-started-with-mysql/mysql-sample-database/) 분석 프로젝트 입니다. 실제 제조업에서 사용하는 데이터베이스 형식을 기반으로, 고객, 주문, 재고, 판매현황, 임직원 등의 정보를 포함하고 있습니다. Python의 mysql.connector 라이브러리를 사용하여 데이터베이스에 직접 연결하고 SQL 쿼리를 실행하여 데이터를 추출한 후, 이를 활용해 10가지 분석 문제를 해결합니다.  
이 프로젝트의 목표는 고객 및 제품 데이터를 체계적으로 분석하여 매출 증대와 고객 맞춤형 마케팅 전략, 재고 최적화 방안 등을 제안하는 것입니다


## 2. 데이터 설명 
- 데이터 출처 : [MySQL의 ClassicModels 샘플 데이터베이스](https://www.mysqltutorial.org/getting-started-with-mysql/mysql-sample-database/)
- 데이터 상세 : 8개 테이블과 59개의 칼럼
  - `customers`: 고객 데이터. 고객 번호, 고객 이름, 연락처 정보 등.
  - `orders`: 주문 데이터. 주문 번호, 주문 날짜, 배송 날짜, 주문 상태 등.
  - `orderdetails`: 각 주문의 상세 데이터. 제품 코드, 주문된 수량, 가격 등.
  - `products`: 판매 제품 데이터. 제품 코드, 제품 이름, 제품 라인, 재고 수량, 구매 가격, MSRP(권장 소매 가격) 등.
  - `productlines`: 제품 라인(카테고리) 데이터. 제품 라인 설명, 제품 라인에 속한 제품들의 이미지 등.
  - `employees`: 회사 직원 데이터. 직원 번호, 직원의 성과 이름, 직위, 상사, 근무 사무실 등.
  - `offices`: 회사 사무실 데이터. 사무실 코드, 사무실 위치, 전화번호, 국가 등.
  - `payments`: 고객의 지불 데이터. 지불 방식, 지불 날짜, 금액 등.

## 3. 분석 과정
1) Vip 고객 식별 [바로가기](https://github.com/Clinda02/market_analysis_with_mysql/blob/main/1_vip_customer_segmentation.ipynb)
2) 고객 충성도 분석과 시각화 [바로가기](https://github.com/Clinda02/market_analysis_with_mysql/blob/main/2_customer_loyalty_analysis.ipynb)
3) 고객 세분화 및 타겟 마케팅 [바로가기](https://github.com/Clinda02/market_analysis_with_mysql/blob/main/3_top_purchased_products_analysis.ipynb)
4) 지역별 매출 분석과 시각화
5) 제품 카테고리 별 매출 분석
6) 가장 잘 팔리는 제품 분석
7) 제품군 별 연도별 매출 추세 분석
8) 재고 최적화 분석
9) 이익 마진 분석 
10) 시즌별 판매 분석

## 4. 필요 라이브러리 
* mysql.connector
* pandas
* matplotlib
* seaborn
