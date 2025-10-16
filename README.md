# 🍔 Delivery-Service

프로젝트 간단 요약 및 소개

- **프로젝트 목적**: 군인 정보 관리와 근무/휴가 일정 시각화로 효율적인 부대 운영 지원  
- **주요 기능**: 군인 인사 정보 등록, 근무/휴가 일정 등록 및 조회, 달력 UI 시각화

---

## 👥 팀원 역할 분담

| 이름 | 역할 | 담당 내용 |
|------|------|-----------|
| 이수현 | 개인 프로젝트 | 군인 정보 관리, 근무/휴가 일정 기능 전반 설계 및 개발 |
| 이수현2 | 개인 프로젝트 | 군인 정보 관리, 근무/휴가 일정 기능 전반 설계 및 개발 |

---

## ⚙ 서비스 구성 및 실행 방법

### 환경 설정 (Prerequisites)
- Java 17 이상, Spring Boot 3.x  
- H2 / MySQL 데이터베이스  
- Node.js (프론트엔드 빌드 시)

### 실행 방법
1. GitHub 레포지토리 클론
   ```bash
   git clone https://github.com/YourUsername/army-management.git
   
## 📌 프로젝트 목적/상세

군인 인사 정보와 소속 부대 관리

날짜 기반 근무/휴가 일정 등록 및 시각화

FullCalendar 기반 달력 UI 연동

군인별 상세 정보 및 근무 내역 조회

## 🗂 ERD

주요 테이블: Soldier, Unit, Schedule

관계: Unit 1:N Soldier, Soldier 1:N Schedule

## 🔧 기술 스택
Back-end

Java, Spring Boot, JPA (Hibernate), QueryDSL

Database

H2, MySQL

Front-end

Thymeleaf, FullCalendar.js

Infra / Tools

Docker (선택), Notion (문서 관리)
