## [ SSAFY 특화 PJT 서울 2반 A204팀 ] Sub 2

### [ 남은 재료 기반 레시피 추천 서비스 ReCook ]

#### 제안 배경
- 코로나19로 인한 외식 감소, 집에서 요리하는 횟수 증가
- 배달 음식의 소비가 증가함에 따라, 남은 음식을 버리게 되어 음식물 쓰레기 증가

#### 서비스 컨셉
- 남은 재료로 만들 수 있는 요리의 레시피를 추천해주는 서비스
- 재료에 맞는 레시피를 일일이 찾아봐야 하는 불편함 해소

#### 기존 서비스와의 차별성
- 기존의 레시피북은 레시피를 확인한 후 재료를 확인했지만,
  이 서비스는 자신이 가진 재료를 통해 만들 수 있는 레시피를 추천해준다
- 유저의 취향을 반영하여 레시피 추천 (국가별 음식 종류 / 알레르기 등)

#### 타겟
- 집에서 남은 재료로 그럴듯한 요리를 만들어 먹고 싶은 사람

#### 기능

- 메인 기능
```
- 남은 재료를 입력하면, 이것으로 만들 수 있는 레시피 추천
- 유저의 취향을 잔뜩 반영한 레시피 / 인기 레시피 / 최신 레시피 추천
- 해당 레시피를 보고 유저가 만든 음식 사진 게시 기능
- 타유저들이 게시한 음식 사진 모아보기 기능
```

- 부가 기능
```
- 조리시간 / 인분 등 제공
- 해당 레시피에 포함된 유저의 알레르기 정보 알림
- 음식 관련 영상 제공
```

#### 필요 기술 스택
- 빅데이터 : Python
- Backend : Spring Boot, MariaDB
- Frontend : Vue.js

#### 빅데이터 이용
- 레시피 크롤링
- 유저들이 많이 이용하는 레시피 / 재료 분석
- 유저의 취향 : 알레르기 정보 / 국가별 음식 선호도 등

#### 고도화
- 개인 취향에 맞는 레시피 추천 서비스 정확도 고도화
- 남은 재료 뿐만 아니라 남은 배달음식으로 만들 수 있는 레시피 추천 서비스
- 재료 사진을 찍으면 어떤 재료인지 인식하고, 레시피를 추천해주는 서비스
- 레시피 동영상 제목을 크롤링해서, 레시피를 글 뿐만 아니라 영상으로도 제공

#### 참고 URL

- 크롤링 방법 :
[PYTHON 크롤링을 이용한 만개의 레시피 크롤링 - 1](https://da-nika.tistory.com/9)

- 공공데이터 농수산물 :
[공공데이터 포털](https://www.data.go.kr/data/15058981/openapi.do)
