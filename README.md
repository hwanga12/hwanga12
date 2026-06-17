# 출시와 성능 개선 경험을 가진 백엔드 엔지니어 황가연입니다.

Spring Boot, Node.js, FastAPI 기반으로 서비스를 구현하며  
반복 조회, 대용량 응답, 캐싱, AI 처리 지연, 배포 흐름에서 발생하는 병목을  
수치로 확인하고 개선해 왔습니다.

- Dayori: App Store / Google Play 출시 서비스 백엔드 개발
- Dayori: 휴지통 조회 API 23.6s -> 0.4s, 전송량 2.6GB -> 54MB 개선
- Playce: 중계 일정 조회 API 12.49s -> 1.16s 개선
- EEUM: 메시지 조회 API 17.21s -> 58.6ms 개선
- 수확행: FastAPI, ROS2, MQTT, YOLOv8 기반 Web-Robot-AI-IoT 흐름 구현

---

# Engineering Highlights

### Performance Optimization
- Dayori에서 DTO Projection, Pageable, 인덱스를 적용해 휴지통 조회 API를 **23.6s -> 0.4s**로 개선
- Playce에서 Redis 캐싱과 캐시 무효화 전략을 적용해 중계 일정 조회 API를 **12.49s -> 1.16s**로 개선
- EEUM에서 JPA N+1 문제를 FETCH JOIN과 페이지네이션으로 개선해 메시지 조회 API를 **17.21s -> 58.6ms**로 개선

### Backend Engineering
- Spring Boot 기반 사용자, 상점, 에셋, 메시지 도메인 API 개발
- PostgreSQL, MongoDB, Redis, S3를 데이터 특성에 따라 분리한 저장 구조 설계
- FastAPI 기반 로봇 관제, AI 추론, IoT 명령 API 구현

### Infra / Reliability
- AWS EC2, RDS, S3 기반 서비스 배포 및 운영 경험
- Docker, Nginx, Jenkins 기반 배포 환경 구성
- k6, Grafana, CloudWatch를 활용한 부하 테스트 및 성능 지표 확인

### AI / Domain Integration
- YOLOv8 기반 병해 진단 결과를 Rule Engine 기반 처방 명령으로 연결
- AI 음성 메시지 처리에서 캐싱과 비동기 처리로 응답 지연 개선
- PyTorch 기반 회귀 모델과 GPT API를 활용한 추천 기능 구현 경험

---

# Tech Stack

### 주력
Java 21 · Spring Boot · JPA · Spring Security  
PostgreSQL · MySQL · Redis  
AWS EC2 · RDS · S3

### 활용 가능
TypeScript · Node.js · Express · TypeORM  
Python · FastAPI · Django REST Framework  
MongoDB · Docker · Nginx · Jenkins · PM2

### 경험
Kotlin · Flutter · Android Studio  
ROS2 · Gazebo · MQTT  
PyTorch · YOLOv8 · GPT API  
k6 · CloudWatch · Grafana · Prometheus · Loki

---

# Project Experience

### Dayori
> 대학생을 위한 올인원 디지털 다이어리 서비스  
> App Store / Google Play 출시 서비스

- 역할: Backend · Infra · 부팀장
- Java 21 · Spring Boot · JPA · PostgreSQL · MongoDB · Redis · AWS S3
- 사용자, 상점, 에셋 도메인 API 설계 및 구현
- PostgreSQL, MongoDB, Redis, S3 기반 저장소 책임 분리
- 휴지통 조회 API 성능 개선: 23.6s -> 0.4s
- 전송량 개선: 2.6GB -> 54MB
- 운영 중인 서비스로 소스코드는 private 관리
- [Portfolio Case Study](노션링크)
- [App Store](앱스토어링크)
- [Google Play](구글플레이링크)

### [EEUM](https://github.com/hwanga12/EEUM)
> 독거노인 안전 모니터링 및 가족 음성 기반 스마트 케어 플랫폼

- 역할: Backend · Infra
- Java · Spring Boot · JPA · MySQL · Redis · Jenkins · Docker · Nginx
- AI 음성 메시지 서버 캐싱 및 비동기 처리 구조 개선
- 메시지 조회 N+1 병목을 FETCH JOIN과 Pageable로 최적화
- 메시지 조회 API 성능 개선: **17.21s -> 58.6ms**
- AI 음성 메시지 응답 개선: **28s -> 670ms**

### [Playce](https://github.com/hwanga12/Playce)
> 위치 기반 실시간 스포츠 중계 식당 검색 서비스

- 역할: Backend · Infra
- TypeScript · Node.js · Express · TypeORM · MySQL · Redis · AWS EC2
- 중계 일정 CRUD, 위치 기반 검색, 통합 검색 API 구현
- Redis 캐싱 및 캐시 무효화 전략 적용
- 중계 일정 조회 API 성능 개선: **12.49s -> 1.16s**
- 통합 검색 API 성능 개선: **1.52s -> 504ms**
