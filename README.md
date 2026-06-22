# 제갈현빈 - Java Full-Stack Developer Portfolio

> 요구사항을 화면설계서와 데이터 흐름으로 분해하고, AI를 보조 도구로 활용해 기술적 근거를 확인하며 구현하는 신입 개발자

## Profile

- Name: 제갈현빈
- Email: Ij941212@naver.com
- Portfolio URL: `https://[GitHub-ID].github.io/[portfolio-repo-name]/`
- GitHub: `https://github.com/[GitHub-ID]`
- 지원 방향: Java 백엔드 / Java 풀스택 신입 개발자

> 공개 포트폴리오에는 상세 주소와 휴대전화 번호를 넣지 않는 것을 권장합니다. 이력서 본문에는 기재하되, 외부 공개 링크에는 이메일과 GitHub 정도만 노출하는 방식이 안전합니다.

## About Me

Java 풀스택 개발자로 성장하기 위해 KOSMO 국비지원 자바 풀스택 개발자 과정을 수강하며 Java, JavaScript, React, TypeScript, Spring Boot, MySQL 기반 웹 개발을 학습하고 있습니다. 대학에서는 발명특허 분야를 학습하며 C, Python, Arduino 기초 코딩과 기술 분석 경험을 쌓았고, 세계 발명 관련 대회에서 팀원들과 함께 금상 2회를 수상했습니다. 현재는 SMU8 티켓팅 홈페이지 프로젝트를 통해 사용자/관리자 UI, 인증/권한 분기, 예매 흐름, 좌석 선택, 결제 프로세스, 데이터베이스 설계, 고트래픽 제어 포인트 분석까지 경험하고 있습니다.


## Development Approach

### 요구사항 우선

AI가 제시한 코드보다 먼저 화면설계서와 Description/Check 내용을 기준으로 고객이 원하는 기능과 흐름을 파악합니다.

### 기술적 근거 확인

REST API 설계, 인증/인가 구조, 계층 분리, DTO 분리 등 실제 개발자들이 문제를 해결하기 위해 정리해 온 원칙과 사례를 확인하며 구현합니다.

### 보안과 예외 처리

JWT role claim, Spring Security 인증 흐름, 사용자/관리자 권한 분기, 예외 메시지, 기존 기능 보존 범위를 함께 고려합니다.

### AI 활용 방식

AI를 단순 코드 생성 도구로 의존하지 않고, 구현 방향을 검토하고 대안을 비교하는 보조 도구로 활용합니다.

## Main Project - SMU8 Ticketing Website

SMU8 티켓팅 홈페이지 프로젝트는 공연 예매 서비스를 주제로 사용자와 관리자 화면을 구현하고, 티켓팅 서비스 특성상 특정 시간대에 트래픽이 집중되는 상황을 고려하여 확장하고 있는 팀 프로젝트입니다. 현재는 Redis를 적용하기 전 단계로 Spring Boot와 MySQL 기반 구조에서 인증, 예매 흐름, 좌석 선택, 결제 프로세스의 기본 구조를 정리하고 있습니다. 이후 Redis를 활용한 대기열, 좌석 임시 선점, rate limit, refresh token blacklist 등을 적용하여 처리 성능과 안정성을 비교할 계획입니다.


### Tech Stack

- **Programming Languages**: Java, JavaScript, TypeScript, HTML5, CSS3, SQL, Python, C
- **Framework / Library**: React, React Router, Spring Boot
- **Server**: Spring Boot, REST API, Spring Security, JWT, 외부 API 연동 구조, Kakao Map API 백엔드 연동
- **Tooling / DevOps**: Git, GitHub, IntelliJ IDEA, VS Code, npm, Vite, Figma, PowerShell, Git Bash
- **Data Base**: MySQL, ERD, IR, 정규화, JOIN, Transaction, Index
- **Environment(OS)**: Windows, Linux 기초
- **ETC**: 화면설계서, 정보구조도, 화면 흐름도, User Flow, 요구사항 분석, REST API 설계 이해, MVC 패턴, DTO/VO 분리, Controller-Service-Repository 구조, Mock Data 테스트 환경, URL parameter 페이지네이션, React Hook 리팩토링, JWT 권한 분기, Spring Security 인증 흐름, 예외 처리 및 보안 흐름 검토, 대기열·좌석 선점·동시성·트래픽 제어 포인트 분석, README 문서화

### Main Responsibilities

- Figma를 활용하여 사용자/관리자 화면설계서, 정보구조도, 화면 흐름도, User Flow 작성
- React와 TypeScript 기반 사용자 메인, 공연 검색, 예매중인공연, 예매임박공연, 공연 상세, 마이페이지, 관리자 공연장 관리 UI 구현
- 예매 대기열, 좌석 선택, 가격 선택, 결제, 예매 완료 흐름에 필요한 Mock Data와 TypeScript 타입 정의
- 공연 검색 Mock Data 통합 및 예매중인 공연/예매임박 공연 필터링, 정렬, 페이지네이션 구조 개선
- URL query parameter 기반 페이지네이션 훅과 통합 검색 훅 구현
- Spring Boot Controller, Service, Repository, DTO 계층 구조 분석 및 HTTP request/response 분리 기준 정리
- JWT role claim을 활용한 일반 사용자/관리자 권한 구분 로그인 흐름 구현
- Redis 적용 전 대기열, 좌석 선점, 동시성 제어, 트래픽 폭주 제어 포인트 분석
- MySQL 기반 ERD 및 IR 설계, 카카오맵 API 백엔드 연동 구조 구현

### Current Stage and Next Plan

SMU8 티켓팅 프로젝트는 현재 Spring Boot와 MySQL 기반의 인증, 예매 흐름, 좌석 선택, 결제 프로세스 구조를 정리하는 단계입니다. 이후 Redis를 적용하여 대기열 처리, 좌석 임시 선점, rate limit, refresh token blacklist 기능을 구현하고, Redis 적용 전후의 처리 성능과 안정성을 비교할 계획입니다. 이를 통해 단순 CRUD 중심의 웹 프로젝트를 넘어, 티켓팅 서비스에서 요구되는 고트래픽 제어와 동시성 문제를 이해하는 방향으로 확장하고자 합니다.


### Learned

- 화면설계서와 기능 명세를 기준으로 구현 범위를 판단하는 방법
- React/TypeScript에서 Mock Data와 타입을 함께 정리하는 방법
- URL query parameter 기반 페이지네이션과 검색 상태 관리
- Spring Boot 계층형 아키텍처와 DTO 분리 기준
- JWT와 Spring Security 기반 인증/권한 분기 흐름
- 티켓팅 서비스에서 대기열, 좌석 선점, 동시성, 트래픽 제어가 필요한 이유
- README 기반 변경 이력 관리와 협업 문서화의 중요성

## Other Projects

### JAVA WIKI

- 설명: Java 학습 내용을 구조화하여 개념을 저장하고 검색할 수 있도록 구성한 개인 프로젝트입니다. 순수 Java 기반으로 데이터 구조와 검색 흐름을 정리하며 Java 문법, 클래스 구조, 검색 로직 구현 경험을 쌓았습니다.
- 기술: Java, Swing GUI, Search Logic, File/Data Structure

### 진로설계 서비스 페이지

- 설명: 레벤슈타인 디스턴스 알고리즘을 활용하여 입력 키워드와 유사한 결과를 추천하는 흐름을 실험한 프로젝트입니다. 문자열 유사도 계산과 사용자 입력 기반 추천 흐름을 학습했습니다.
- 기술: Java, Levenshtein Distance, Search/Recommendation Logic

## Awards and Background

- 세계 발명 관련 대회 금상 2회 수상
- 발명특허 분야 학습 경험: 특허, 실용신안, 민법, 특허법 등
- KOSMO 국비지원 Java 풀스택 개발자 과정 수강 중

## Resume Portfolio Field Example

```text
포트폴리오: https://[GitHub-ID].github.io/[portfolio-repo-name]/
GitHub: https://github.com/[GitHub-ID]
프로젝트 저장소: https://github.com/[GitHub-ID]/smu8-ticketing
```
