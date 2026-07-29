# [황가연] Backend · DevOps

### 데이터 설계 역량:
올인원 다이어리 'Dayori' - PostgreSQL·MongoDB·Redis·S3 데이터 성격에 맞게 사용, DTO Projection 인덱스를 적용 하여 휴지통 조회 API 응답 시간 (23.6초 -> 0.4초) 개선 경험

### 성능 튜닝 역량:
스포츠 중계 지도 서비스 'Playce' - Redis 캐시 키 설계·인증 흐름 개선 (중계 일정 조회 12.49초 -> 1.16초)
스마트 헬스 케어 서비스 'EEUM' - JPA N+1을 Fetch Join으로 해결(메시지 조회 17.21초 58.6ms)

### DevOps 역량:
스마트 헬스 케어 서비스 'EEUM' - AWS EC2·RDS·S3 운영 환경 구축, Jenkins로 FE/BE 배포 분리 및 Docker 이미지 정리, k6 부하 테스트 Grafana·Prometheus·Loki 모니터링



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
- [App Store](https://apps.apple.com/kr/app/dayori-%EB%8B%A4%EC%9D%B4%EC%96%B4%EB%A6%AC-%EC%BA%98%EB%A6%B0%EB%8D%94-%ED%95%84%EA%B8%B0/id6764240658)
- [Google Play](https://play.google.com/store/apps/details?id=com.dayori.app&pcampaignid=web_share)

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
