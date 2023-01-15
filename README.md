# 피마 당뇨병 환자 분류 문제
1. 데이터 셋 확인
2. EDA
3. 특성 공학(Feature Engineering)
4. 모델 개발 및 학습
5. 모델 예측 및 평가

### 1. 데이터 셋 확인
- 데이터가 어떻게 구성되어 있는 지 확인한다.
- 결측치는 존재하지 않는다.

1. Pregnancies : 임신 횟수
2. Glucose : 포도당 부하 검사 수치
3. BloodPressure : 혈압
4. SkinThinkness : 팔 삼두근 뒤쪽의 피하지방 측정값
5. Insulin : 혈청 인슐린
6. BMI : 체질량 지수
7. DiabetesPedigreeFunction : 당뇨 내력 가중치 값
8. Age : 나이
9. Outcome : 클래스 결정 값

### 2. EDA
- 데이터가 어떤식으로 분포되어 있는 지 적절한 시각화를 통해서 분석한다.
- 연속형 데이터가 많아서 kde 그래프를 주로 활용하였다.
- 포도당, 혈압, 피하지방, BMI, 나이는 당뇨병에 어느 정도 영향을 주는것으로 보인다.
- 혈청 인슐린은 당뇨병 환자가 당뇨병이 아닌 사람보다 낮은 경향을 보여주고 있다.
- Correlation 그래프를 통해 상관관계를 확인한다.
- 히스토그램을 통해 각 칼럼별 분포도 확인한다.

### 3. Feature Engineering
- Glucose에 5개, BloodPressure에 35개, SkinThickness에 227개, Insulin에 374개, BMI에 11개가 0으로 결측치가 존재했다.
- Glucose 결측치는 제거하고 나머지 칼럼의 결측치는 평균으로 대체했다.


### 4. 모델 개발 및 학습
- Standard Scaler로 스케일링 한다.
- 로지스틱 회귀 모델로 학습시켰다.
- 임계값을 변화시키면서 학습해봤다.

### 5. 모델 학습 결과 (kaggle 제출 기준)




