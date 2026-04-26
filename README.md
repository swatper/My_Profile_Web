# 💻 404_NotFound: Personal Portfolio Web
> **NCP(Naver Cloud Platform) 기반의 동적 콘텐츠 관리가 가능한 개인 포트폴리오 웹 사이트**

## 1. 개요
- **기술 스택**: HTML5, CSS3, JSP, MySQL, Naver Cloud Platform
- **핵심 목표**: 데이터베이스 중심의 동적 UI 구현 및 클라우드 기반 안정적 서비스 배포

## 2. 주요 기능
### 🌐 1. 클라우드 인프라 구축 및 배포
- **Naver Cloud Platform (NCP)** Micro 인스턴스 활용
- **환경 구성**: Linux(CentOS) 환경에서 Apache Tomcat 9 WAS 구축
- **버전 관리**: Git을 활용한 서버-로컬 간 소스코드 관리 및 배포 프로세스 정립
- **실시간 수정**: VI 편집기를 활용한 서버 환경 설정 및 긴급 코드 대응

### 🛠 2. Project 섹션: 데이터베이스 기반 동적 콘텐츠
- **동적 렌더링**: JSP와 MySQL을 연동하여 DB에 저장된 정보를 실시간으로 화면에 출력
- **데이터 구조 설계**:
  - 프로젝트 기본 정보와 이미지 경로(Path)를 별도 테이블로 관리 (1:N 관계 처리)
  - **구분자 활용**: 스킬 스택 및 세부 설명을 하이픈(`-`) 문자로 구분하여 저장 후, 출력 시 파싱하여 UI 최적화
- **데이터 전송**: HTML Form의 `POST` 메서드를 통한 데이터 적재 시스템 구현

### ✉️ 3. Message 섹션: 방문자 소통 창구
- 사용자가 남긴 메시지를 DB에 영구 저장하는 데이터 파이프라인 구축
- 프로젝트 섹션과 동일한 POST 전송 방식을 사용하여 데이터 무결성 확보

## 4. 개발 환경
- **IDE**: VSCode (Remote-SSH), VI Editor
- **Terminal**: PuTTY (SSH 원격 접속 및 서버 제어용)
- **Server**: Naver Cloud Platform (Micro Instance)
- **WAS**: Apache Tomcat 9.0
- **DB**: MySQL
