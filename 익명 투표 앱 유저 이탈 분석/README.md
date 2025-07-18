# 익명 투표 앱 유저 이탈 분석과 전환 유도 방안
---------
## 1. 분석 주제 : 
익명 칭찬 투표 ‘H’어플은 출시 후 2달만에 앱스토어 1위, 일 가입자 5만명을 달성하였으나, 이후 빠르게 감소하는 신규 가입자와 높은 유저 이탈률이 발생

-----
## 2. 분석 목표 :
30만 유저의 로그기록을 분석하여 이탈의 주된 원인을 분석하고 유저 이탈률 최소화 방안을 탐색하여 최적의 마케팅 인사이트를 도출

-----
## 3. 데이터셋 :
| 데이터 소스       | 파일 형식 | 수집 기간                 | 활용 목적               |
|------------------|-----------|--------------------------|------------------------|
| Hackle 데이터     | Parquet   | 2023.07.11 ~ 2023.08.04 | EDA, 유저 행동 분석     |
| Hackle 데이터     | JSON      | 2023.06.18 ~ 2023.09.04 | EDA, 유저 행동 분석     |
| votes 데이터      | SQL       | 2023.03.29 ~ 2024.05.09 | EDA, 질문 추천 개선     |
------
## 4. 분석 인프라 :
| 항목                   | 내용                                                                 |
|----------------------|----------------------------------------------------------------------|
| 클라우드 환경         | • GCP VM (e2-standard-16: vCPU 16개, RAM 64GB)  <br>  ○ CPU: AMD Rome (x86/64)  <br>  ○ OS: Linux (VM 환경) |
| 데이터 저장           | MySQL (VM 서버 내)                                                   |
| 데이터 추출 및 작업 툴 | VSCode (SSH 원격 접속)                                                |
| Python 버전           | Python 3.12.7                                                        |


