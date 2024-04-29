# U.STRA Framework

GSITM에서 운영 중인 U.STRA Framework 공식 Release Repository 입니다.

## 공지 사항

### 공식 가이드 안내

공식 가이드 사이트 : http://guide.ustraframework.kro.kr/

현재 공식 가이드는 일부 기능을 제한적으로 운영 중에 있습니다. 다음 기능이 제한됩니다.

- 데모 서비스
- 공지사항

문의 사항은 [이슈](https://github.com/ustraframework/ustraframework/issues)로 등록해 주시기 바랍니다.


### 공식 의존성 저장소 변경 안내

GSITM 전사 자원 정책 변경으로 의존성 저장소를 변경할 예정입니다.

현재는 임시 저장소를 제공하고 있으니 참고하기 바랍니다.

- 메이븐 레파지토리 : http://repo.ustraframework.kro.kr/repository/maven-public/
- NPM 레지스트리 : http://repo.ustraframework.kro.kr/repository/npm-public/


## Release Note (Java)

### 2.3.0 RELEASE (2024/04/04)

U.STRA Java Framework 2.3.0은 2024년 4월 4일에 릴리즈되었습니다.

2.3.0 버전에는 다음과 같은 변경 사항이 적용됩니다.

#### 신규 기능

- 메시지 기능
- 텍스트 템플릿 기능
- 데이터 지원 유틸리티 추가
- H2 데이터베이스 연계 기능 추가

#### 기능 개선

- 메뉴 관리 / 프로그램 아이디 값 검증 추가
- 파일 그룹 관리 / 파일 유형 제한 기능 추가
- 권한 관리 / 권한 사용 기간 설정 개선
- 배치 관리 / 배치 작업 실행 이력 조회 조건 개선
- 인터페이스 관리 / 인터페이스 관리 기능 개선

#### 결함 수정

- UstraException 메시지 생성 시 불필요한 포맷팅이 발생하는 오류 수정
- Oracle 페이지네이션 처리 시 카운트 쿼리를 잘못 만드는 오류 수정
- 파일 그룹의 파일명 형식을 원본 파일명 + 순번 + 확장자로 지정하는 경우 업로드에 실패하는 오류 수정
- 파일 등록 시 FileId 생성 전 FileAccessUrl을 만드는 오류 수정
- 메뉴 이동 시 메뉴 단계가 변경되지 않는 오류 수정
- MySQL을 사용하는 경우 사용 기간 만료 배치의 만료 주기가 잘못 적용되는 오류 수정

#### 업그레이드 방법

2.2.1 버전에서 2.3.0 버전으로 업그레이드 시 다음 작업이 필요합니다.

1. 일부 테이블이 변경되었습니다. 데이터베이스 별로 다음 쿼리를 실행해 주세요.

```sql
-- Oracle
ALTER TABLE USTRA_IFS ADD LMT_YN CHAR(1) DEFAULT 'N' NULL;
UPDATE USTRA_IFS SET LMT_YN = 'N';
COMMENT ON COLUMN USTRA_IFS.LMT_YN IS '제한_여부'
-- SQL Server
ALTER TABLE USTRA_IFS ADD LMT_YN CHAR(1) DEFAULT 'N' NULL;
UPDATE USTRA_IFS SET LMT_YN = 'N';
EXEC sp_addextendedproperty 
	@name=N'MS_Description', @value=N'제한_여부', 
	@level0type=N'SCHEMA', @level0name=N'dbo', 
	@level1type=N'TABLE', @level1name=N'USTRA_IFS'
	@level2type=N'COLUMN', @level2name=N'LMT_YN'
-- PostgreSQL
ALTER TABLE USTRA_IFS ADD COLUMN LMT_YN CHAR NULL;
UPDATE USTRA_IFS SET LMT_YN = 'N';
COMMENT ON COLUMN USTRA_IFS.LMT_YN IS '제한_여부';
-- MySQL / MariaDB
ALTER TABLE USTRA_IFS ADD COLUMN LMT_YN CHAR DEFAULT 'N' NULL COMMENT '제한_여부' AFTER USE_YN;
-- H2
ALTER TABLE USTRA_IFS ADD LMT_YN CHAR(1) DEFAULT 'N' NULL
UPDATE USTRA_IFS SET LMT_YN = 'N';
COMMENT ON COLUMN USTRA_IFS.LMT_YN IS '제한_여부';
```

2. `build.gradle` 또는 `pom.xml` 파일에서 프레임워크 버전을 `2.2.1.RELEASE`에서 `2.3.0.RELEASE`로 변경해 주세요.


## Release Note (Node)

### 2.0.35-stable (2021/10/6)

백오피스 엑셀 다운로드 페이징 동기화 처리

UrlBuiler 기능 추가


## Release Note (Nexacro)
### 1.0.3 (2021/10/07)

그리드 연계 기능 추가

Axios 통신 라이브러리 업데이트

팝업 표준화

입력 샘플 추가

<!--
**ustraframework/ustraframework** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
