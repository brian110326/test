#  🚚📦 ShoongLogistics B2B MSA Project

프로젝트 간단 요약 및 소개

- **프로젝트 목적**: ShoongLogistics는 단순한 주문.배달 서비스에서 나아가 기업 간 물류 관리와 배송 프로세스를 운영할 수 있는 MSA 기반 플랫폼을 목표로 개발되었습니다.
- **주요 기능**: 회원 인증.인가(JWT 기반), 주문 및 배달 관리, 허브 및 업체 관리
- **개발 기간**: 2025/10/31 ~ 2025/11/13

---

## 📌 프로젝트 목적 / 상세

### 1. 회원 서비스
- 역할(Role) 기반 인증/인가(MASTER, HUB_MANAGER, COMPANY_MANAGER, SHIPPER 등)
- JWT 토큰 발급 및 유효성 검증
- Spring Security 기반 세션 무관 인증 구조

### 2. 허브 서비스
- 중앙 허브(CENTRAL) 및 일반 허브(NORMAL) 관리
- 허브별 위치(위도/경도) 기반 관리
- 허브 간 이동 경로 간 최적화

### 3. 주문 및 배달 서비스
- 주문 생성 및 상태 관리
- 배달자 자동 매칭
- 허브 간 물류 이동 경로 관리

### 4. 업체 및 상품 서비스
- 업체 등록(MANUFACTURER, RECEIVER 구분)
- 허브 기반 업체 소속 관리
- 상품 등록/수정/삭제 관리
- 재고 관리

### 5. 알림 서비스
- Slack Webhook 기반 실시간 알림
- 주문 생성 시 알림 전송
- AI 기반 응답 메세지 작성

---

## 👥 팀원 역할 분담

| 이름 | 역할 | 담당 내용                                                |
|------|------|------------------------------------------------------|
| 강태성 | 팀장 |Jwt 기반 인증/인가 구현, 이메일 인증 시스템, 인프라 설계, 배포 자동화      |
| 이나라힘 | 테크리더더 | 리뷰/답글 API 구현, 리뷰 조회 Redis 캐싱, Spring AI를 활용한 답글 자동생성 |
| 김다애 | 팀원 | 주소 API, PostGIS를 활용한 가게 조회, S3 Presigned URL         |
| 이수현 | 팀원 | 지역(시·도, 시·군·구, 동) API, AI 프롬프트 API, Slack API        |

---

## ⚙ 서비스 구성 및 실행 방법

### 환경 설정 (Prerequisites)
- Java 17 이상
- Spring Boot 3.5.6 이상
- PostgreSQL 16 이상
- Gradle 8.8 이상
- Redis 8.2.2 이상

### 실행 방법

```
./gradlew clean build -x test
java -jar build/libs/backend-0.0.1-SNAPSHOT.jar
java -jar build/libs/*.jar
```
---

## 🗂 ERD

<img width="2973" height="1615" alt="Image" src="https://github.com/user-attachments/assets/8722a581-f1b9-4289-8c68-f05b38fb5f04" />

---

## 📄 API 문서

[Swagger 링크] : http://localhost:8000/swagger-ui/index.html

---

## 🔧 기술 스택
### Back-end
- **Java**
- **Spring Boot**
    - Spring Security
    - Spring AI
    - JWT
    - JUnit
    - QueryDSL
    - Lombok
    - Actuator
- **JPA (Hibernate)**

### Database
- PostgreSQL(with PostGIS)

### Infrastructure
- Docker
- Grafana
- nGrinder
- Redis
- Prometheus

### CI/CD
- Github Actions를 이용해 PR 시 자동 빌드 및 테스트 실행
- dev 브랜치 병합 전 코드 품질을 검증하도록 설정

### Tools
- Github
- Figma
- Erd Cloud
- Postman
- Swagger
- Slack
- Notion

