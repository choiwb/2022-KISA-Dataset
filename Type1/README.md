# Type1 디지털 트윈 기술을 이용한 IT 서비스 보안 관제용 AI 데이터 셋

<br>

### Type1 개요
-----
##### 1. IT 서비스 모사 및 시뮬레이션 환경 구성
IT 서비스 모델을 벤치마킹한 시뮬레이션 환경에 공격자를 능동적으로 유인하기 위한 허니팟 등의 유인기법을 적용한다. IDS/IPS 및 Firewall 장비 등 이기종 보안장비 5종 이상을 구축하며, 공격 탐지, 호스트 로그 및 트래픽 등 각종 보안로그 수집 및 분석 기능이 포함된다. 또한, 정상 이용자 행위 10종 이상이 설계 및 수행된다.
##### 2. 모사환경 타깃 위협탐지 및 보안로그 수집/가공
공격 유인을 통해 SQL 인젝션, 스캐닝, 로그인 시도, 정보탈취 등 위협 행위를 탐지하고, 탐지된 위협을 20종 이상의 유형으로 분류한다. 또한, 위협별 보안로그를 분석하여 ATT&CK 프레임워크에 제시된 공격전술(T-ID)을 식별한다. 공격 트래픽(pcap), 정상/공격 네트워크 및 호스트 이벤트 로그 및 이기종 보안장비 5종 이상의 이벤트 로그를 수집한다.

<br>

### Type1 망구성도
-----
![image](https://user-images.githubusercontent.com/44902157/218399684-ab176b81-a5d3-4a6f-a275-35485f8cf18e.png)

<br>

### 데이터 정의
-----
##### 1. 원시데이터: 시나리오의 공격 재현에 따라 생성된 데이터
##### 2. 원천데이터: 공격에 따라 발생되는 데이터를 수집/정제
##### 3. 라벨데이터: 정제된 데이터에 라벨 추가

<br>

### 데이터 수 요약
-----
|장비|원시데이터|원천데이터|라벨데이터|
|------|------|------|------|
|FW|[125,124,863](https://github.com/choiwb/2022-KISA-Dataset/blob/d965c76df0ad9919549997b4176327e3aeef7a96/Type1/%EC%9B%90%EC%8B%9C%EB%8D%B0%EC%9D%B4%ED%84%B0/%EC%9E%A5%EB%B9%84%EB%B3%84/1-FW-RAW.csv)|125,124,863|125,113,969|
|IPS|[45,195](https://github.com/choiwb/2022-KISA-Dataset/blob/d965c76df0ad9919549997b4176327e3aeef7a96/Type1/%EC%9B%90%EC%8B%9C%EB%8D%B0%EC%9D%B4%ED%84%B0/%EC%9E%A5%EB%B9%84%EB%B3%84/1-IPS-RAW.csv)|45,195|45,195|
|IDS|[121,766](https://github.com/choiwb/2022-KISA-Dataset/blob/d965c76df0ad9919549997b4176327e3aeef7a96/Type1/%EC%9B%90%EC%8B%9C%EB%8D%B0%EC%9D%B4%ED%84%B0/%EC%9E%A5%EB%B9%84%EB%B3%84/1-IDS-RAW.csv)|121,766|121,766|
|WAF|[89,116](https://github.com/choiwb/2022-KISA-Dataset/blob/d965c76df0ad9919549997b4176327e3aeef7a96/Type1/%EC%9B%90%EC%8B%9C%EB%8D%B0%EC%9D%B4%ED%84%B0/%EC%9E%A5%EB%B9%84%EB%B3%84/1-WAF-RAW.csv)|89,116|89,116|
|WEB_NginX|[14,069,567](https://github.com/choiwb/2022-KISA-Dataset/blob/d965c76df0ad9919549997b4176327e3aeef7a96/Type1/%EC%9B%90%EC%8B%9C%EB%8D%B0%EC%9D%B4%ED%84%B0/%EC%9E%A5%EB%B9%84%EB%B3%84/1-WEB_NginX-RAW.csv)|14,069,567|13,477,124|
|데이터 합계|139,450,507|139,450,507|138,847,170|

<br>

### 행위별 데이터 수
-----
[Type1_행위별데이터수.xlsx](https://github.com/choiwb/2022-KISA-Dataset/blob/a20c783a8aa6566dbf7bf84db0b22a493722152f/Type1/Type1_%ED%96%89%EC%9C%84%EB%B3%84%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%88%98.xlsx) 파일 참고
