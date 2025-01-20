# 부동산 허위매물 탐지 프로젝트

이 프로젝트는 부동산 허위매물을 탐지하기 위한 머신러닝 모델을 개발하는 것을 목표로 합니다.

## 주요 기능

- 데이터 전처리 및 분석
- 머신러닝 모델 학습 및 평가
- 데이터 시각화

## 사용된 라이브러리

- pandas: 데이터 처리 및 분석
- numpy: 수치 연산
- scikit-learn: 모델 학습 및 평가
- seaborn, matplotlib: 데이터 시각화
- imblearn: 데이터 불균형 문제 해결
- lightgbm: 머신러닝 모델

## 데이터셋

- train.csv: 학습 데이터
- test.csv: 테스트 데이터

## 주요 코드 설명

1. 필요한 라이브러리 임포트
2. 데이터 로드
3. 타겟 변수 분포 확인 및 시각화
4. 데이터 전처리 (추정)
5. 모델 학습 및 평가 (추정)

## 사용 방법

1. 필요한 라이브러리 설치
2. train.csv와 test.csv 파일을 준비
3. 코드 실행

## 주의사항

- 한글 폰트 설정이 필요할 수 있습니다 (MacOS 기준 AppleGothic 사용)
- 데이터 불균형 문제가 있으므로 SMOTE 기법을 사용하여 해결합니다

## 향후 개선 사항

- 모델 성능 개선
- 추가적인 특성 엔지니어링
- 다양한 모델 비교 실험

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/40228632/0a19d11b-6d18-43a1-9534-f434a1ca4235/real_estate_fraud_3.ipynb
