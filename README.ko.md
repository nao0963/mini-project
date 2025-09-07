# 비건 소셜 플랫폼 - `풀잎당`

[🇺🇸 English](README.md) | 🇰🇷 한국어

비건 애호가들을 소셜 피드, 카페 예약, 그룹 활동, 커뮤니티 토론을 통해 연결하는 종합 비건 커뮤니티 플랫폼입니다.

## 📝 프로젝트 개요

**목적**: 비건들이 경험을 공유하고, 비건 친화적인 카페를 발견하며, 모임을 조직하고, 커뮤니티 토론에 참여할 수 있는 전용 소셜 플랫폼 구축

**대상 사용자**: 연결, 정보, 공유 경험을 추구하는 비건 커뮤니티 구성원

**핵심 기능**:
- **사용자 로그인** → 개인화된 사용자 경험을 위한 안전한 계정 생성 및 로그인
- **비건 피드** → 비건 경험과 라이프스타일 콘텐츠의 SNS 스타일 공유
- **카페 예약** → 서울의 비건 디저트 카페 발견 및 예약
- **그룹 활동** → 비건 중심의 모임 조직 및 참여
- **커뮤니티 게시판** → 비건 주제에 대한 열린 토론 포럼

## 🔧 기술 스택

### 🛠️ 백엔드
- **언어**: Java
- **프레임워크**: Spring Boot
- **ORM**: 데이터베이스 통합 및 매퍼 구성을 위한 MyBatis
- **아키텍처**: 계층화된 서비스 아키텍처를 가진 MVC 패턴

### 🎨 프론트엔드
- **핵심 기술**: HTML5, CSS3, JavaScript
- **UI/UX**: 모던 스타일링을 가진 반응형 웹 디자인
- **템플릿 엔진**: 서버 사이드 렌더링을 위한 Thymeleaf

### 🗄️ 데이터베이스
- **데이터베이스**: 데이터 저장 및 관리를 위한 MySQL
- **데이터 모델링**: 정규화된 구조를 가진 관계형 데이터베이스 설계

### ⚙️ 개발 도구
- **버전 관리**: 협업 및 코드 저장소를 위한 GitHub
- **IDE**: 백엔드 개발 환경을 위한 IntelliJ IDEA
- **빌드 도구**: 의존성 관리 및 빌드 자동화를 위한 Gradle

## 📁 프로젝트 구조

```
vegan-social-platform/
├── src/main/java/com/playdata/miniproject/
│   ├── board/                    # 게시판 기능
│   │   ├── controller/          # 게시판 컨트롤러
│   │   ├── dao/                 # 데이터 접근 객체
│   │   ├── dto/                 # 데이터 전송 객체
│   │   ├── mapper/              # MyBatis 매퍼
│   │   └── service/             # 비즈니스 로직 서비스
│   ├── cafe/                    # 카페 예약 시스템
│   │   ├── controller/          # 카페 컨트롤러
│   │   ├── dao/                 # 카페 데이터 접근
│   │   ├── dto/                 # 카페 DTO
│   │   ├── mapper/              # 카페 매퍼
│   │   └── service/             # 카페 서비스
│   ├── community/               # 그룹 커뮤니티 기능
│   │   ├── controller/          # 커뮤니티 컨트롤러
│   │   ├── dao/                 # 커뮤니티 데이터 접근
│   │   ├── dto/                 # 커뮤니티 DTO
│   │   ├── mapper/              # 커뮤니티 매퍼
│   │   └── service/             # 커뮤니티 서비스
│   ├── feed/                    # 소셜 피드 기능
│   │   ├── controller/          # 피드 컨트롤러
│   │   ├── dao/                 # 피드 데이터 접근
│   │   ├── dto/                 # 피드 DTO
│   │   ├── mapper/              # 피드 매퍼
│   │   └── service/             # 피드 서비스
│   ├── user/                    # 사용자 관리
│   │   ├── controller/          # 사용자 컨트롤러
│   │   ├── dao/                 # 사용자 데이터 접근
│   │   ├── dto/                 # 사용자 DTO
│   │   ├── mapper/              # 사용자 매퍼
│   │   └── service/             # 사용자 서비스
│   ├── config/                  # 설정 클래스
│   └── util/                    # 유틸리티 클래스
├── src/main/resources/
│   ├── mappers/                 # MyBatis XML 매퍼
│   ├── static/                  # 정적 웹 리소스
│   │   ├── css/                 # 스타일시트
│   │   ├── js/                  # JavaScript 파일
│   │   └── images/              # 이미지 자산
│   └── templates/               # Thymeleaf 템플릿
└── build.gradle                # 빌드 설정
```

## 🌟 핵심 기능

### 1. 사용자 인증 및 프로필 관리
![사용자 페이지](vegan-social-platform/images/User_page_1.png)

- 안전한 사용자 등록 및 로그인 시스템
- 비건 선호도가 포함된 개인화된 사용자 프로필
- 계정 관리 및 개인정보 설정

### 2. 비건 소셜 피드
![피드 페이지](vegan-social-platform/images/Feed_page_1.jpg)

- 비건 라이프스타일 경험과 레시피 공유
- 소셜 상호작용이 포함된 사진 및 텍스트 기반 게시물
- 좋아요와 댓글을 통한 커뮤니티 참여
- 개인 피드 관리 및 콘텐츠 큐레이션

### 3. 비건 카페 발견 및 예약
![카페 및 예약](vegan-social-platform/images/C&R_page_1.png)

- 서울의 비건 디저트 카페 종합 디렉토리
- 가용성 확인이 포함된 실시간 예약 시스템
- 메뉴, 위치, 리뷰를 포함한 카페 정보
- 사용자를 위한 통합 예약 관리

### 4. 커뮤니티 그룹 및 모임
![그룹 페이지](vegan-social-platform/images/Group_page_1.png)

- 비건 중심의 관심 그룹 생성 및 참여
- 지역 모임 및 이벤트 조직
- 그룹 토론 게시판 및 활동 계획
- 멤버 관리 및 참여 추적

### 5. 토론 게시판
![게시판 페이지](vegan-social-platform/images/Board_page_1.png)

- 비건 관련 토론을 위한 열린 포럼
- 주제 분류 및 검색 기능
- 조정 기능이 포함된 사용자 생성 콘텐츠
- 지식 공유 및 커뮤니티 지원

## 🚀 시작하기

### 필수 조건
- Java 11 이상
- MySQL 8.0+
- Gradle 7.0+
- IntelliJ IDEA (권장)

### 설치

1. 저장소 복제:
```bash
git clone <repository-url>
cd vegan-social-platform
```

2. 데이터베이스 설정 구성:
```bash
# MySQL 구성으로 application.properties 업데이트
cp src/main/resources/application.properties.example src/main/resources/application.properties
```

3. 애플리케이션 빌드 및 실행:
```bash
./gradlew bootRun
```

4. 애플리케이션 접근:
```
http://localhost:8080
```

## 👥 팀 멤버

[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/YunSHCode) **윤성훈** - 풀스택 개발 (게시판/커뮤니티)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/nao0963) **김선영** - 데이터베이스 설계 및 백엔드 개발 (유저)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/05Daul) **김다울** - 프론트엔드 개발 및 통합 (카페)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/netioz) **김민지** - 프론트엔드 개발 및 UI/UX (피드)

## 📊 데이터베이스 설계

### 개체-관계 다이어그램
<img src="vegan-social-platform/src/main/resources/static/images/ERD.png" alt="ERD 다이어그램" width="80%">

데이터베이스 설계는 다음을 지원합니다:
- 사용자 인증 및 프로필 관리
- 콘텐츠 생성 및 소셜 상호작용
- 시간 데이터가 포함된 예약 시스템
- 그룹 멤버십 및 활동 추적

## 📋 문서

### 프로젝트 명세서
- [기능 명세서](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1791406220#gid=1791406220)
- [요구사항 명세서](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1670477596#gid=1670477596)

### 테스트 결과
- [프론트엔드 테스트 결과](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1518302369#gid=1518302369)
- [백엔드 테스트 결과](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=475843754#gid=475843754)

## ✨ 기술적 하이라이트

### 아키텍처 설계
- **MVC 패턴**: 컨트롤러, 서비스, 데이터 접근 계층의 명확한 관심사 분리
- **RESTful API**: 프론트엔드-백엔드 통신을 위한 표준화된 HTTP 엔드포인트
- **반응형 디자인**: 크로스 디바이스 호환성을 보장하는 모바일 우선 접근법

### 보안 기능
- 사용자 인증 및 세션 관리
- 입력 검증 및 SQL 인젝션 방지
- 사용자 생성 콘텐츠를 위한 안전한 파일 업로드 처리

### 성능 최적화
- MyBatis를 사용한 데이터베이스 쿼리 최적화
- 정적 리소스 캐싱 및 압축
- 효율적인 이미지 처리 및 저장

## 🔮 향후 개선사항

- **모바일 애플리케이션**: 네이티브 iOS 및 Android 앱
- **실시간 알림**: 커뮤니티 활동을 위한 푸시 알림
- **고급 검색**: AI 기반 콘텐츠 발견 및 추천
- **통합 API**: 서드파티 비건 레스토랑 및 제품 데이터베이스
- **국제화**: 글로벌 비건 커뮤니티를 위한 다국어 지원

---

*이 팀 프로젝트는 Java Spring Boot를 사용한 웹 개발의 기초를 연습하기 위해 만들어졌습니다.*