# 황가연 | Java/Spring Backend Developer

Java와 Spring Boot로 백엔드 API를 개발하고 Redis 캐시 정합성과 배포 흐름을 개선해 왔습니다. 또 부하 테스트에서 휴지통 조회 시간을 23.6초에서 0.4초로 줄인 경험이 있습니다.

AI 에이전트에 기존 코드와 API 규칙을 제공해 기능을 구현하고 오류를 분석했습니다. 구현 결과는 로그와 테스트로 확인했습니다.

Dayori에서는 백엔드 개발과 인프라를 맡고 부팀장으로서 팀 일정을 조율하며 앱 출시와 운영까지 참여했습니다.

## Core Stack

Java 21 · Spring Boot · Spring Security · JPA  
PostgreSQL · MySQL · MongoDB · Redis  
AWS · Docker · Nginx · Jenkins · JUnit · k6

---

## Project Experience

### Dayori

> 일정·필기·에셋 마켓을 통합한 대학생 디지털 다이어리  
> App Store·Google Play 출시  
> 운영 중인 서비스로 소스코드는 비공개로 관리하고 있습니다.

- **6인 팀 / Backend·Infra / 부팀장** — 사용자·상점·에셋 API와 PostgreSQL·MongoDB·Redis·S3 저장 구조 설계
- DTO Projection·페이지네이션·인덱스를 적용해 k6 50VU의 동일 요청 횟수 기준 휴지통 조회 평균 응답 시간 **23.6초 → 0.4초**, 전송량 **2.6GB → 54MB**로 개선
- AI 에이전트와 탈퇴·복구 인증 흐름을 분석해 기존 토큰 재사용 문제를 발견하고, 토큰 무효화 정책과 JUnit 회귀 테스트 적용

[App Store](https://apps.apple.com/kr/app/dayori-%EB%8B%A4%EC%9D%B4%EC%96%B4%EB%A6%AC-%EC%BA%98%EB%A6%B0%EB%8D%94-%ED%95%84%EA%B8%B0/id6764240658) · [Google Play](https://play.google.com/store/apps/details?id=com.dayori.app)


---

### [EEUM](https://github.com/hwanga12/EEUM)

> 독거노인 안전 모니터링 및 가족 음성 기반 스마트 케어 플랫폼

- **6인 팀 / Backend·Infra** — 메시지·알림 기능 개발 및 Spring Boot 서버와 AI 음성 서버 연계
- Fetch Join으로 메시지 조회의 N+1 문제를 해결하고 20건 단위 페이지네이션 적용
- Jenkins의 FE·BE 배포 단계를 분리하고 미사용 Docker 이미지 정리 절차 구성

---

### [Playce](https://github.com/hwanga12/Playce)

> 위치와 경기 일정을 기반으로 스포츠 중계 식당을 찾는 지도 서비스

- **6인 팀 / Backend·Infra** — 중계 일정 CRUD, 위치 기반 검색 및 복합 검색 API 구현
- Redis 캐시 키와 무효화 범위를 설계해 동일 요청 횟수 기준 중계 일정 조회 평균 응답 시간 **12.49초 → 1.16초**로 개선
- 검색 쿼리와 조회 구조를 개선해 통합 검색 평균 응답 시간 **1.52초 → 504ms**로 단축
