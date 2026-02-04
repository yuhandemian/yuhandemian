<h1 align="center">Hi, I'm Yuhan Park 👋</h1>

I’m diving deep into **backend development**, focusing on scalable and high-performance systems.  
Recently, I’ve been exploring distributed system design to understand how large architectures behave under load.

---

### 📬 Contact
[Email](mailto:yuhn1011@naver.com) ｜ [LinkedIn](https://www.linkedin.com/in/yuhanpark12345/)

---

### 🛠️ Tech Stack

**Backend** <br>
<img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white">
<img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"><br>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white">

**Database & Cache** <br>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white">
<img src="https://img.shields.io/badge/MongoDB-47A248.svg?&style=for-the-badge&logo=MongoDB&logoColor=white">
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=Redis&logoColor=white">

**Infra** <br>
<img src="https://img.shields.io/badge/DOCKER-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white">
<img src="https://img.shields.io/badge/AWS%20RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white">
<img src="https://img.shields.io/badge/AWS%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white">
<img src="https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white">  

<br>

---
### 🚀 Projects

#### 🎬 모두의 플리
- **Period**: 2025.12 – 2026.01  
- **Role**: Team Lead /Backend Developer  
- **Tech**: Spring Boot, JPA, QueryDSL, Redis, MySQL, AWS ECS, Docker, Prometheus, Grafana  
- **Highlights**:
  - Prometheus·Grafana 기반 서비스 모니터링 구성
  - **Concurrency Control: Subscriber Count Race Condition**
  - 구독자 수 증가 시 Race Condition 발생
  - RDBMS Row-level Lock 기반 `UPDATE count = count + 1` 원자적 연산으로 해결
  - ms 단위 대기 시간으로 정합성 100% + 높은 처리 성능 확보

- **Query Optimization: Cursor Pagination & Subscription Lookup**
  - 플레이리스트 목록·구독 조회 쿼리 성능 저하 문제 확인
  - 정렬 기준(UpdatedAt / SubscriberCount / CreatedAt) 기반 복합 인덱스 설계
  - 평균 응답시간 **90.3% 감소**, P99 **91.6% 감소**
  - TPS **35.8% 증가**, Tail Latency 개선

- **Hotspot Mitigation in Read-Heavy Traffic**
  - Read:Write ≈ 100:1 환경에서 특정 플레이리스트로 트래픽 집중
  - Zipfian 분포 기반 부하 테스트로 Hotspot 재현
  - Redis Cache-Aside 패턴 적용 (Miss 시 DB 조회 후 캐싱)
  - Playlist Detail API 평균 응답시간 **46.3% 감소**,  
    P99 **22.2% 개선**, TPS **2.57% 향상**
- 🔗 [GitHub](https://github.com/codeit-mopl)

---

#### 🤖 미어캣AI
- **Period**: 2025.03 – 2025.09 
- **Role**: Team Lead / Backend Developer  
- **Tech**: Spring Boot, FastAPI, MySQL, AWS, Nginx  
- **Highlights**:
  - 실시간 AI 추론 서버(FastAPI)와 Spring Boot 백엔드 분리 설계
  - RTSP 연동 실환경에서 추론 정확도 저하 문제 발생
  - CCTV 입력(30fps)과 모델 학습 데이터(3fps) 간 프레임 레이트 불일치 원인 규명
  - Frame Sampling Filter 설계로 입력 시계열을 학습 데이터 기준에 동기화
  - 실환경에서도 테스트 환경과 유사한 추론 정확도 확보
- 🔗 [GitHub](https://github.com/Capstone-project-team7) | [Demo](https://meerkatai.shop/)

---

#### 📰 모뉴
- **Period**: 2025.10 – 2025.11  
- **Role**: Team Lead / Backend Developer  
- **Tech**: Spring Boot, Spring Batch, JPA, Redis, PostgreSQL, MongoDB, AWS ECS, S3, Docker  
- **Highlights**:
  - Spring Batch 기반 뉴스 수집 자동화 (OpenAPI, RSS)
  - Redis 조회수 중복 방지 및 장애 대비 Fallback 로직
  - AWS S3 연동 일일 뉴스 데이터 백업·복구 시스템
  - GitHub Actions 기반 CI/CD 파이프라인 구축
- 🔗 [GitHub](https://github.com/codeit-monew)

---

#### 📊 Findex
- **Period**: 2025.09  
- **Role**: Backend Developer  
- **Tech**: Spring Boot, JPA, QueryDSL, PostgreSQL, Docker
- **Highlights**:
  - 지수 조회·필터·정렬 API 및 성과 랭킹 로직 구현
  - 이동평균선·가격 변동 비교 데이터 가공 및 CSV 다운로드
- 🔗 [GitHub](https://github.com/codeit-projects-5th/Findex)
---

### 💎 Achievements

- **🏆 2025 SW중심대학 우수작품 경진대회 — 우수상(소프트웨어중심대학 협의회장상)**  

미어캣AI: AI 기반 무인점포 이상행동 감지 시스템  

- **주최**: 과학기술정보통신부  
- **주관**: IITP(정보통신기획평가원), SW중심대학협의회  
- **참여 규모**: 전국 58개 대학 대표팀  
- **출전**: 세종대학교 대표  
- **역할**: 팀장 / 백엔드 개발

#### 🔗 References
- [**대회 수상 결과**](https://www.swuniv.kr/72/?bmode=view&idx=168784681)
- [**프로젝트 소개 공식 Ebook (p.56)**](https://bypub.kr/ebook/msit2025A/index.html#p=56)
- [**GitHub Repository**](https://github.com/Capstone-project-team7)
- [**Service Demo**](https://meerkatai.shop/)

> 🔐 **Demo Account**  
> - This service provides a demo account for evaluation purposes.  
> - Demo credentials are available upon request.  

- **🥇 Top Prize(1st Place): 『2025년 세종대학교 제19회 창의설계경진대회』 19th Sejong University Creative Engineering Design Competition**  
  → [**MeerkatAI**: Unmanned Store Abnormal Behavior Detection System using AI](https://github.com/Capstone-project-team7)  
  → Team Lead & Backend Developer
  
### 📰 Media Coverage

- **[SW중심대학 10주년] 전국 58개 대학 SW 우수작품 경진대회**
  - 세종대학교 대표 팀 *MeerkatAI*, 우수상(SW중심대학협의회장상) 수상
  - ETNews, 2025.11.27
  - 🔗 [기사 링크](https://www.eduplusnews.com/news/articleView.html?idxno=16946)
 
- **구윤철 부총리, 세종대 AI 역량강화 현장 방문**
  - 현장 실습 프로젝트로 *MeerkatAI*를 소개하고 시스템 설명을 진행함
  - NewsPim, 2025.12.18  
  - 🔗 [기사 링크](https://m.news.nate.com/view/20251218n22731)
---

### 🌱 Education
- **SEJONG UNIVERSITY — B.S. Computer Engineering** (Mar 2023 – Aug 2025)

### 📘 Professional Training
- **Codeit Sprint — Backend Developer Program** (Jul 2025 – Jan 2026)
