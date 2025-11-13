#  🚚📦 ShoongLogistics B2B MSA Project

프로젝트 간단 요약 및 소개

- **프로젝트 목적**: ShoongLogistics는 B2B 기반 배달 관리 플랫폼으로 
- **주요 기능**: 주문, 리뷰, 가게 관리와 회원 인증/인가, AI 답글, 캐시, 알림 기능을 지원하는 백엔드 서비스
- **개발 기간**: 2025/10/31 ~ 2025/11/13

---

## 📌 프로젝트 목적 / 상세

### 1. 회원 서비스
- 역할(Role) 기반 인증/인가 구현
- JWT 토큰 발급 및 유효성 검증
- 회원 정보 조회/수정/삭제

### 2. 허브 서비스
- 기능

### 3. 주문 및 배달 서비스
- 기능

### 4. 업체 및 상품 서비스
- 기능

### 5. 알림 서비스
- 기능

---

## 👥 팀원 역할 분담

| 이름 | 역할 | 담당 내용                                                |
|------|------|------------------------------------------------------|
| 이나라힘 | 팀장 |Jwt 기반 인증/인가 구현, 이메일 인증 시스템, 인프라 설계, 배포 자동화      |
| 이수현 | 팀원 | 리뷰/답글 API 구현, 리뷰 조회 Redis 캐싱, Spring AI를 활용한 답글 자동생성 |
| 갇태성 | 팀원 | 주소 API, PostGIS를 활용한 가게 조회, S3 Presigned URL         |
| 김다애 | 팀원 | 지역(시·도, 시·군·구, 동) API, AI 프롬프트 API, Slack API        |

---

## ⚙ 서비스 구성 및 실행 방법

### 환경 설정 (Prerequisites)
- Java 17 이상
- Spring Boot 3.5.6 이상
- PostgreSQL 16.10(Ubuntu) 이상
- Gradle 8.8 이상
- Redis 8.2.2 이상
- Spring AI 1.0.3 이상

### 실행 방법

```
./gradlew clean build -x test
java -jar build/libs/backend-0.0.1-SNAPSHOT.jar
java -jar build/libs/*.jar
```
---

## 🗂 ERD

<img width="1000" height="1000" alt="image" src="https://github.com/user-attachments/assets/d651e969-9b17-499a-a615-15eec76ca1d8" />

---

## 📄 API 문서

[Swagger 링크] : http://43.203.27.160/swagger-ui/index.html

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
- **JPA (Hibernate)**

### Database
- PostgreSQL(with PostGIS)

### Infrastructure
- **Google AI Studio**
- Docker

### CI/CD
- Github Actions

### Tools
- Github
- Figma
- dbdiagram.io
- Postman
- Swagger
- Slack
- Notion

