# 💳 Woori Card Data Analyzing: 광고 노출 최적화 프로젝트
| **Install ELK in ubuntu and practice ELK using Woori card data**
<br></br>

## 👨‍👨‍👦‍👦 Team

👥 팀명 : 구구구칠

|<img src="https://avatars.githubusercontent.com/u/87555330?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/55776421?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/71498489?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/82265395?v=4" width="150" height="150"/>|
|:-:|:-:|:-:|:-:|
|김민성<br/>[@minsung159357](https://github.com/minsung159357)|SeulGi_LEE<br/>[@seulg2027](https://github.com/seulg2027)|HanJH<br/>[@letsgojh0810](https://github.com/letsgojh0810)|구민지<br/>[@minjee83](https://github.com/minjee83)|


## 🎯 프로젝트 목표
모바일 채널의 광고 노출 빈도를 효율적으로 조절하여 고객 소비 증대
</br>
</br>
## 🔍 핵심 아이디어
### 1. 데이터 세분화 전략
- 인구통계학적 분석
  - 나이별 소비 패턴
  - 지역별 소비 트렌드
  - 라이프스테이지별 소비 특성

### 2. 채널 맞춤 광고 전략
비대면 채널 가입자

- 앱 푸시 광고 노출
- 개인화된 타겟팅

비대면 채널 미가입자

- SMS 문자 광고 발송
- 가입 유도를 위한 연회비 인센티브 제공
</br>

## 📊 인프라 및 아키텍처
### ELK 스택 구축
- Elasticsearch
- Logstash
- Kibana
</br>

<img src="./img/architecture.png" width="550">

## 🛠 주요 기술
- 데이터 수집
- 데이터 처리
- 시각화
- 인사이트 도출
</br>

<br></br>
# 👀 Hands On
# 📊 우리카드 소비 데이터 분석 인사이트

## 1. 데이터 시각화 개요
소비자 세분화를 위한 6가지 데이터 분석 관점

### 📈 분석 차원
1. 나이별 소비 패턴
2. 지역별 소비 트렌드 
3. 라이프스테이지별 소비 특성

## 2. 고객 세분화 전략

### 🎯 채널별 마케팅 접근법
- **비대면 채널 가입자**: 앱 푸시 광고 
- **비대면 채널 미가입자**: SMS 문자 광고
  - 가입 인센티브: 연회비 절감

## 3. 데이터 인사이트 상세

### 3.1 나이별 소비 분석
#### 연령대별 주요 소비 분야
<img src="https://github.com/user-attachments/assets/9b538d23-7e8c-4c7e-b57a-438a0c02b08b" width="500">

| 연령대 | 주요 소비 분야 |
|--------|----------------|
| 20대 | - 온라인 쇼핑<br>- 외식<br>- 여행 |
| 30대 | - 육아용품<br>- 교육<br>- 생활용품 |
| 40대 | - 자녀 교육<br>- 가전제품<br>- 보험 |
| 50대 | - 의료서비스<br>- 여행<br>- 자기계발 |
| 60대 이상 | - 의료<br>- 건강관리<br>- 생활용품 |

### 3.2 지역별 소비 트렌드
#### 주요 지역 특성
<img src="https://github.com/user-attachments/assets/509ce11c-1ccb-4152-8637-566a0acb3e80" width="500">

| 지역 | 주요 소비 특성 |
|------|----------------|
| 서울 | - 고급 소비재<br>- 문화생활 |
| 경기 | - 실용적 소비<br>- 가족 중심 지출 |
| 부산 | - 해운/관광 관련 소비 |
| 대구 | - 전통시장<br>- 지역 중소기업 제품 |
| 제주 | - 관광/여행 관련 소비 |

### 3.3 라이프스테이지별 소비 특성
<img src="https://github.com/user-attachments/assets/e832b7c2-3278-445a-af42-d6a3f321dcde" width="500">

## 라이프스테이지별 소비 특성 분석

| 라이프스테이지 | 주요 소비 분야 | 마케팅 포인트 |
|--------------|--------------|--------------|
| 대학생 | - 교육<br>- 온라인 쇼핑 | - 학생 할인<br>- 청년 특화 상품 |
| 신혼/영유아 부모 | - 육아용품<br>- 가전제품 | - 육아 관련 금융 서비스 |
| 자녀 학령기 부모 | - 교육<br>- 학원비 | - 교육 관련 금융 상품 |
| 사회초년생 | - 자기계발<br>- 문화생활 | - 취업/자격증 대출 |
| 은퇴/시니어 | - 건강관리<br>- 여행 | - 건강보험<br>- 은퇴 설계 |

### 3.4 비대면 채널 가입 여부
## 나이별 가입 여부
<img src="https://github.com/user-attachments/assets/10911534-f130-4645-8196-ee58dedb8d00" alt="나이별 가입 여부" width="500">

## 지역별 가입 여부
<img src="https://github.com/user-attachments/assets/22a3d241-29ec-43df-8ea9-a67ab2022a71" alt="지역별 가입 여부" width="500">

## 라이프스타일별 가입 여부
<img src="https://github.com/user-attachments/assets/d9502fb5-3a85-4ede-bcf1-bd1b25832e98" alt="라이프스타일별 가입 여부" width="500">



## 4. 마케팅 전략 제안

### 🚀 채널별 맞춤 접근
1. 비대면 채널 가입자
   - 개인화된 앱 푸시 광고
   - 실시간 맞춤형 혜택 제공

2. 비대면 채널 미가입자
   - SMS 타겟 광고
   - 채널 가입 유도 인센티브
     * 연회비 절감
     * 초기 가입 혜택

## 💡 5. 기대 효과
- 타겟팅 정확도 향상
- 고객 경험 최적화
- 광고 효율성 증대
- 데이터 기반 마케팅 전략 수립
