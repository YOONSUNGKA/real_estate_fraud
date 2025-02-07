# 부동산 사기 예측 (4번째 모델)

## 📌 개요
이 프로젝트는 머신러닝 기법을 활용하여 부동산 사기를 예측하는 것을 목표로 합니다. 데이터에는 다양한 부동산 속성과 거래 정보가 포함되어 있으며, 모델의 성능은 F1-score를 기준으로 최적화됩니다.

## 📂 프로젝트 구조
```
├── real_estate_fraud_4.ipynb   # 주요 주피터 노트북 파일
├── train.csv                   # 학습 데이터셋
├── test.csv                    # 테스트 데이터셋
├── README.md                   # 프로젝트 문서 (이 파일)
├── requirements.txt            # 필요한 패키지 목록
└── output/                     # 예측 결과 저장 폴더
```

## 🚀 설치 방법
1. 저장소를 클론하거나 노트북 파일을 다운로드합니다.
2. 필요한 라이브러리를 설치합니다:
   ```bash
   pip install -r requirements.txt
   ```

## 📊 방법론
이 노트북은 다음과 같은 순서로 실행됩니다:
1. **데이터 로딩 및 전처리**
   - `train.csv` 및 `test.csv` 불러오기
   - ID 컬럼 제거
   - KNN Imputer를 사용한 결측값 보완
   - 범주형 변수 인코딩 (라벨 인코딩 및 원-핫 인코딩 적용)
   
2. **데이터 불균형 처리**
   - SMOTE (Synthetic Minority Over-sampling Technique) 적용
   
3. **모델 학습**
   - LightGBM을 활용한 머신러닝 모델 학습
   - Stratified K-Fold 교차 검증 (5-Fold) 적용
   - GridSearchCV를 이용한 최적 하이퍼파라미터 탐색
   
4. **평가 및 예측**
   - F1-score를 기반으로 모델 평가
   - `test.csv`에 대한 최종 예측 수행

## 📈 모델 성능
- 모델 성능은 F1-score 평가 기준을 따릅니다.
- 목표: **높은 F1-score 달성 및 모델 일반화 성능 개선**

## 🛠 사용 방법
1. `real_estate_fraud_4.ipynb`를 Jupyter Notebook 또는 Google Colab에서 엽니다.
2. 모든 셀을 순차적으로 실행합니다.
3. 최종 예측 파일이 `output/` 폴더에 저장됩니다.

## 📌 향후 개선 사항
- 하이퍼파라미터 튜닝을 통한 모델 성능 개선
- 추가적인 특징 공학(feature engineering) 기법 적용
- 다양한 모델 앙상블을 통한 성능 향상

## 🔗 참고 자료
- [Scikit-learn 공식 문서](https://scikit-learn.org/)
- [LightGBM 공식 문서](https://lightgbm.readthedocs.io/)

