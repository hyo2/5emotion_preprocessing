# 5emotion_preprocessing
2022.07 5emotion data 전처리

## 진행환경
- colab

## 데이터
- 분류되는 감정을 <분노, 슬픔, 놀람(당황), 중립, 기쁨> 총 5가지로 결정함
- 총 67217개의 데이터-각 감정별로 약 13,000~13500개의 데이터 사용

## 사용한 데이터셋
- 'AI 허브'에서 제공하는 데이터셋 총 3가지를 주제에 맞춰 수정하여 사용함
  1. 한국어 감정 정보가 포함된 단발성 대화 데이터셋
  2. 한국어 감정 정보가 포함된 연속성 대화 데이터셋
  3. 감성대화 말뭉치
     
1. 단발성 및 연속성 대화 데이터셋
- 공포, 놀람, 분노, 슬픔, 중립, 행복, 혐오 총 7가지의 감정으로 분류되어 있음
- 필요한 데이터만 추출해서 사용함
2. 감성대화 말뭉치
- 분노, 슬픔, 당황, 상처, 불안, 행복의 6가지 기본 감정을 기준으로 각각 9개의 세부 감정이 포함된 60개 감정 상태가 반영된 문장으로 이루어진 데이터셋
- 이중 이러한 감정이 드러나도록 문장을 생성한 첫번째 발화만 사용
- ‘당황’, ‘충격 받은’, ‘당혹스러운’의 내용인 것을 선별하여 ‘놀람’ 으로 새로 레이블링하여 사용함

## 요약
- 데이터 확인, 읽기, 정제, 수집, 저장
- 전처리: 한글만 남기기, 맞춤법 및 띄어쓰기 교정, 반복문자 정제
