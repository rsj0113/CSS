# CSS
CSS (Credit Scoring System)


> **1. EDA (1_Home_Credit_Default_Risk_EDA.ipynb)**

1.1. Kaggle 데이터 가져오기

(application_test.csv.zip	    installments_payments.csv.zip
application_train.csv.zip	    bureau_balance.csv.zip		    POS_CASH_balance.csv.zip
bureau.csv.zip			    previous_application.csv.zip    credit_card_balance.csv.zip)

1.2. Pandas 데이터프레임 생성 및 데이터 구조 파악

(train, test, bureau, bureau_balance)

1.3. Feature Engineering

train : key (SK_ID_CURR distinct)

test : key (SK_ID_CURR distinct)

bureau : key (SK_ID_BUREAU distinct), SK_ID_CURR 중복

bureau_balance : SK_ID_BUREAU 중복

Merge 하기 위해서 SK_ID_CURR 기준으로 요약정보 생성하기


1.3.1. Bureau 숫자형 데이터 요약정보 생성

1.3.2. Bureau 문자형 데이터 요약정보 생성

1.3.3. bureau_balance 숫자형 데이터 요약항목 생성

1.3.4. bureau_balance 문자형 데이터 요약항목 생성


1.4. 탐색적 데이터 분석 (EDA)


1.4.1. target 분석


1.4.2. Features 분석

1.4.2.1. 결측치 분석

1.4.2.2. feature 통계량 분석

1.4.2.3. 이상치 조정


1.5. 결합데이터 feature engineering 2


1.6. 결합데이터 Target Correlation


1.7. Feature Selection

1.7.1. Correlation을 이용한 Selection

1.7.2. Feature Importance를 이용한 Selection


1.8. 최종 train, test set 반출



> **2. 모델링 과정**

2.1. 모델링용 데이터 가져오기


2.2. 데이터 전처리

2.2.1. 결측치 처리 ( 0으로 대체 )

2.2.2. 결측치 처리 ( median 으로 대체 )


2.3. 데이터 Split (개발용 & 검증용)

2.4. 모형 학습

2.4.1. 모형학습1 (결측 0으로 대체)

2.4.2. 모형학습2 ( median 으로 대체 )

2.4.3. 모형학습3 ( SMOTE 를 이용한 Oversampling )


> **3. 모형 검증 및 평가**

3.1. K-Fold Cross Validation

3.2. 정오분류표(Confusion Matrix) 통한 검증

3.3. ROC Curve 산출

3.4. 스코어 산출 및 등급화


> (번외) Logistic Regression 을 이용한 Scorecard 산출

1. 데이터 가져오기

2. Binning 

3. Linear 파라미터 설정

4. 스코어카드 생성

5. 스코어카드 반출






