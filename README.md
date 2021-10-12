# U.STRA Framework
GSITM에서 운영 중인 U.STRA Framework 공식 Release Repository 입니다.
- 공식 가이드 사이트 : http://guide.ustraframework.kro.kr/

# Release Note (Java)

## 2.0.41 RELEASE (**2021/10/6**)

웹 소켓 기능 확장

넥사크로 공통 기능 추가 (메뉴 관리)

서블릿 컨트롤러 JSON 문자열 매핑 기능 추가

백 오피스 엑셀 변환 기능 페이징 조건 동기화

CommonDataStore, CommonDataApplicationListener, ObjectFieldsDataMapper
@ConditionalOnMissingBean 추가

PaginationRequest Order null일 경우 오류 발생 패치

이메일 마스킹 유틸리티 오류 패치

배치 개선

- Worker 수용량 기능 추가
- Worker 설정 변경 시 즉시 적용
- Manager 변경 시 동작 추가

## 2.0.40 RELEASE (2021/9/29)

백 오피스 엑셀 다운로드 마스킹 처리

## 2.0.39 RELEASE (2021/9/28)

Release 오류로 재배포

## 2.0.38 RELEASE (2021/9/28)

ustra-data에 Automation Metadata Generation 사용

백오피스 권한 관리 저장방식 일괄 처리로 변경 : 퍼포먼스 개선

중복 인증 폴링 방식 개선 : 중복 스케쥴러 방지

1.0 버전 마이그레이션 보정 기능 이관

## 2.0.37 RELEASE (2021/9/24)

백 오피스 세션 인증 기본 설정 추가

프레임워크 버전 정보 추가 / 배너 변경

API 요청 헤더 값 : HTTP 헤더 리딩 처리

커스톰 REST API 결과 매핑 구조 변경

REST API XML 매핑 구조 변경

## 2.0.36 RELEASE (2021/9/23)

인터페이스 메소드 정보 NULL 오류 보정 처리

넥사크로 Date, LocalDate, LocalDateTime 파라메터 송수신 처리

백 오피스 로그인 이력 시퀀스 채번 (오라클)

## 2.0.35 RELEASE (2021/9/16)

엑셀 변환 오류 제거

DataToExcelWebResourceConverter 추가

사용자 권한 저장 오류 수정

## 2.0.34 RELEASE (2021/9/15)

폴링 체크 쓰레드 큐 사이즈 증가

## 2.0.33 RELEASE (2021/9/15)

UstraExcelUtils 저장 메소드 추가

넥사크로 제네릭 파라메터 타입 매핑 기능 추가

## 2.0.32 RELEASE (2021/9/15)

IP ADDRESS 기반 중복 로그인 체크 쿼리 오류 패치

넥사크로 JSON Object 매핑 기능 추가

## 2.0.31 RELEASE (2021/9/13)

2factor 인증 키 발행 여부 판단 기능 추가

JEUS 웹 소켓 구동 오류 수정

## 2.0.30 RELEASE (2021/9/9)

넥사크로 파라메터 매핑 버그 수정

## 2.0.29 RELEASE (2021/9/9)

Management Bo 프로퍼티 매핑 오류 수정

웹 소켓 기능 추가

JWT 인증 실시간 중복 인증 확인, 자동 로그아웃 처리 기능 추가

UstraSpringTest 시 BasePackage 설정 오류 개선 : 마이바티스 Mapper 조회 불가 현상 개선

NexacroResultBuilder 추가

Profile 추가 문자 설정 프로퍼티 추가

## 2.0.28 RELEASE (2021/9/2)

넥사크로 공통 코드 Controller 생성

넥사크로 파라메터 매핑 버그 수정

## **2.0.27 RELEASE (**2021/**8/25)**

개인정보 처리 시스템 - 사용자 권한 이벤트 수정(권한그룹 수정시에만 이벤트 발생)

사용자 이력, 사용자권한이력 쿼리 수정

mng-bo properties 추가 : 사용자 부서코드 셀렉트박스 사용 여부(useUserDeptCodeSlelctBox)

## **2.0.26 RELEASE (**2021/**8/24)**

파일 그룹 트랜잭션 오류 수정

개인정보 처리 시스템 - 사용자 권한 이벤트 추가

## 2.0.25 RELEASE (2021/8/23)

배치 기능 추가

파일 연계 기능 추가

파일 text 변환 encodeCharset추가

게시 관리 쿼리 수정

## 2.0.24 RELEASE **(**2021/**8/19)**

게시 관리 트랜잭션 오류 수정

zip 파일 다운로드 기능 오류 수정

엑셀 일자 변환 포맷 수정

로그인 이력, 인터페이스 이력, 권한 이력 검색 기간 수정

넥사크로17 프레임워크 기능 추가

메뉴 아이콘 추가

## 2.0.23 RELEASE **(**2021/**8/12)**

프론트 Static 어플리케이션 글로벌 예외 처리 로직 수정

웹 응답 완료 쿠키 : 인터셉터 → 필터 처리 변경

## 2.0.22 RELEASE **(**2021/**8/11)**

파일 연계기능 추가 (파일업로드, 이미지 변환, 엑셀 변환, text변환, 첨부파일 다운, 미리보기)

- text 리소스 변환, 첨부파일 zip다운 기능 제외

## 2.0.21 RELEASE **(**2021/**8/9)**

RestInterfaceTemplate 예외 처리

## 2.0.20 RELEASE **(**2021/**8/9)**

Refresh / 로그인 토큰 사용 시 중복 체크 로직 변경

백오피스 2factor 인증 컨트롤러 추가

Mybatis Mapper Location 제외 패턴 설정 기능 추가

RestInterfaceTemplate callWithHeader 메소드 추가 (헤더 반환 처리 옵션)

Permission 어노테이션 채널별 권한 체크 기능 추가

## 2.0.19 RELEASE **(**2021/**7/28)**

인터페이스 모듈 IP 체크 오류 수정

## 2.0.18 RELEASE **(**2021/**7/26)**

Security ignore 설정 시, Permission 확인 제외 처리

RestInterfaceTemplate Type reference 오류 패치

Static Page View 서버 오류 처리

TextValues Validator 추가

Thymeleaf Template 기능 추가

## 2.0.17 RELEASE **(**2021/**7/22)**

이벤트 기능 추가

전역 권한 체크 시, 인증 완료 여부 체크 추가

bo 인터페이스 로깅 오류 수정

JEUS 구동 오류 수정

bo 게시관리 오류 수정

bo 게시그룹관리 오류 수정

## 2.0.16 RELEASE **(**2021/**7/19)**

REST Header 추가 프로퍼티 설정

페이징 요청 NULL인 경우, Default 설정으로 변경 처리

Validation Group 추가 (CrudGroups)

## 2.0.15 RELEASE **(**2021/**7/16)**

메일 발송 기능 추가

HttpParameterJwtAuthenticationStore 추가 : 파라메터로 토큰 수신 기능

2Factor 인증 프로세스 추가

JEUS WAS 프로퍼티 파일 리딩 오류 현상 개선

JEUS 어플리케이션 메인 클래스 조정

## **2.0.14 RELEASE (**2021/**7/6)**

인증 사용자 조회 캐시 기능 추가

UstraExcelCellInfoModel을 사용해서 다운로드 구현 시 UstraExcelCellType 지정 기능 추가

Mybatis Pagination JEUS WAS 오류 수정

Redis 연계 기능 추가 (캐시, Redis Repository, JWT 리프레시 토큰 저장소)

어플리케이션 추가 설정 파일 적용 로직 수정

## **2.0.13 RELEASE (**2021/**6/29)**

마이바티스 페이징 처리 시 connection 오류 보정

## **2.0.12 RELEASE (**2021/**6/28)**

페이징 처리 시, connection 유지 현상 개선

아웃바운드 인터페이스 샘플 추가

mng-bo 배치 이력 페이징 추가

## **2.0.11 RELEASE (**2021/**6/22)**

BO 토큰 appender 사용자 명 매핑 수정

ServletApplicationRunner 누락 설정 적용

## **2.0.10 RELEASE (**2021/**6/18)**

BO JWT 기본 인증 처리 프로세스 : 확장 가능 구조로 변경

## **2.0.9 RELEASE (**2021/**6/18)**

Static 파일 검증 로직 오류 수정

## **2.0.8 RELEASE (**2021/**6/16)**

리소스 요청 인터페이스 로깅 범위 제외 처리 : ResourceWebInterfaceLoggingFilter

Jeus Mybatis 인터셉터 구동 오류 패치

management 이력 리스트 조회 오류 수정

## **2.0.7 RELEASE (**2021/**6/10)**

XmlResourceInterfaceInfoProvider : XML 리소스 기반 인터페이스 정보 제공 기능 추가

인터페이스 클라이언트 로깅 기능 추가

## **2.0.6 RELEASE (**2021/**6/9)**

jwt인증 : 익명 인증 스토어 비저장 처리

로그아웃 로깅 추가 (BO)

UstraApplicationRequestWrapper: application/x-www-form-urlencoded 지원 처리

mybatis 기본 설정 추가 - jdbcTypeForNull: NULL

## **2.0.5 RELEASE (**2021/**6/7)**

페이징 기능 개선

인바운드 인터페이스 로깅 적용

쿼리 로깅 적용

## **2.0.4 RELEASE (**2021/**6/3)**

Bo 연계 기능 개선

인증 및 권한 모듈 구조 일부 개선

## **2.0.3 RELEASE (**2021/**6/1)**

Bo 연계 기능 추가

Static 유형  프로파일 추출 기능 추가

프로퍼티 암호화 키 파일 조회 기능 추가

프로퍼티 파일 우선 순위 처리 Fix

ProcedureManager 데이터소스 지정 오류 수정

DefaultUstraUserDetailChecker 비밀번호 체크 로직 수정

## **2.0.2 RELEASE**

ProcedureManager

1. callSp 파라미터 추가 (useCaseInsensitive : caseInsensitive Map 사용 여부, default true)
2. callSp 버그 FIX (CURSOR가 없는 경우 resultSet mapper 추가하지 않도록 수정)

## **2.0.1 RELEASE**

Security 구조 변경 : Custom 권한 체크 로직 추가

## **2.0.0 RELEASE**

최초 RELEASE : 1.0 버전 리패키징


# Release Note (Node)

## **2.0.35-stable (2021/10/6)**

백오피스 엑셀 다운로드 페이징 동기화 처리

UrlBuiler 기능 추가

## **2.0.34-stable (2021/9/29)**

백 오피스 엑셀 다운로드 마스킹 처리

## **2.0.33-stable (2021/9/28)**

nuxt-dx-mng-bo : 백오피스 로그인 오류 반환 처리 개선

백 오피스 캐시 제거 시, 자동 로그아웃 처리 수행

API 요청 헤더 값 : HTTP 헤더로 전환 처리

백 오피스 IE11 CSS 오류 수정

백 오피스 관리 화면 오류 및 엑셀 다운로드 파일 명 변경

## **2.0.32-stable (2021/9/27)**

테스트 배포

## **2.0.31-stable (2021/9/17)**

nuxt-dx-mng-bo : 공통 코드 컴포넌트 필터 항목 추가

## **2.0.30-stable (2021/9/15)**

IE 파일 다운로드 오류 개선

## **2.0.29-stable (2021/9/15)**

인증 실시간 폴링 구동 오류 개선

인증 폴링 시간 10초로 변경

## **2.0.28-stable (2021/9/13)**

u-code-select-box 항목 미존재 시 value 값 초기화 처리

## **2.0.27-stable (2021/8/26)**

프로파일 STRAGING ⇒ stg  추가, PRODUCTION ⇒ env 추가

## **2.0.26-stable (2021/8/25)**

파일 다운로드 원복/ 파일 resultData watch설정 추가

사용자 이력, 사용자권한이력 회사명, 부서명 코드매핑 추가

개인정보 팝업 수정

mng-bo properties 추가 : 사용자 부서코드 셀렉트박스 사용 여부(useUserDeptCodeSlelctBox)

## **2.0.25-stable (2021/8/24)**

파일 다운로드 수정

## **2.0.24-stable (2021/8/23)**

백오피스 즐겨찾기 실시간 적용 처리

배치 기능 추가

파일 연계 컴포넌트 개선

즐겨찾기 수정

bo- 게시그룹 수정

bo - 마스킹 수정

권한 서비스 수정

## **2.0.23-stable (2021/8/19)**

파일 다운로드 방식 변경

메뉴 아이콘 추가

## **2.0.22-stable (2021/8/12)**

백 오피스 파일 다운로드 경로 context path 추가

모바일 브릿지 인바운드 요청 로직 개선

## **2.0.21-stable (2021/8/11)**

파일 연계 컴포넌트 개선(파일업로드, 이미지 변환, 엑셀 변환, text변환, 첨부파일 다운, 미리보기)

- text 리소스 변환, 첨부파일 zip다운 기능 제외

## **2.0.20-stable (2021/8/9)**

session, local storage context path 기준 변경

백오피스 컴포넌트 변경 기능 추가

모바일 브릿지 storage 연계 오류 수정

기본 빌드 옵션 조정 (build.extractCSS = false) : CSS Ordering 무시 현상 개선

## **2.0.19-stable (2021/7/26)**

백 오피스 navigation 스토어 구조 변경

## **2.0.18-stable (2021/7/26)**

Vuetify Modal, Gnb 상태 관리 기능 추가

Back Office 사이드 메뉴 선택 이벤트 중복 오류 처리

## **2.0.17-stable(2021/7/26)**

nuxt 2.15.7 버전 업그레이드

서버 미들웨어 : 서버 데이터 연동 기능 추가

- devDependency 수정 필요

```json
{
	"@nuxt/types": "2.15.7",
	"@nuxt/typescript-build": "2.1.0",
	"@nuxtjs/eslint-config-typescript": "6.0.1",
	"@nuxtjs/eslint-module": "3.0.2",
	"@nuxtjs/eslint-config": "3.1.0"
}
```

- .eslintrc rule 추가

```json
{
	"rules": {
    "no-use-before-define": "off"
  }
}
```

## **2.0.16-stable (2021/7/19)**

Devextreme alert/confirm 창 오픈 시 auto focus 기능 추가

Storage 데코레이터 initValue 프로퍼티 추가 : 스토리지 연계 store 초기 값 설정

Back Office : 설정 어플리케이션 (메뉴/코드/설정 정보 리로드 기능 추가)

## **2.0.15-stable (2021/7/15)**

module option configName 추가

## **2.0.14-stable (2021/7/13)**

모바일 브릿지 storage 무한 루프 현상 개선

백오피스 즐겨찾기 기능 추가

백오피스 메뉴 구조 변경

## **2.0.13-stable (2021/7/7)**

플러그인 라우터 기능 추가

플러그인 캐시 핸들링 기능 추가

## **2.0.12-stable (2021/7/6)**

BO Context Path 리소스 적용

## **2.0.11-stable (2021/6/28)**

권한 커스톰 체크 모듈 옵션 추가

resource 경로 변경 (_nuxt ⇒ _ustra)

nuxt-dx-mng-bo 메뉴 일괄변경 오류 수정

nuxt-dx-mng-bo 배치 이력 페이징 추가

## **2.0.10-stable(2021/6/22)**

bo-auth-module 사용자 매핑 override 기능 분리

bo 기본 화면 사용자 데이터 반영 오류 수정

SSR 캐시 기능 적용 (dependency 업데이트 필요)

## **2.0.9-stable(2021/6/18)**

Vue 컴포넌트 예외 처리 로직 수정

SASS 관련 의존 라이브러리 버전 변경

## **2.0.8-stable(2021/6/16)**

u-alert 컴포넌트 with, height prop 추가

UstraBoComponent 마스킹 기능 추가

nuxt-mng-bo 마스킹 글로벌 옵션 추가

bo-auth-module 권한 저장 storage 변경

## **2.0.7-stable (2021/6/15)**

백오피스 공통 데이터 캐시 연계 기능 추가

## **2.0.6-stable (2021/6/10)**

모바일 브릿지 연계 기능

인터페이스 관리 기능 추가

## 2.0.5-stable (**2021/**6/7)

시스템 공통컴포넌트 명칭 변경 ustra 태깅

시스템 공통 메뉴, 비밀번호 로직 수정

## **2.0.4-stable (2021/6/3)**

인증 모듈 개선 버전

Buefy 모듈 추가

BO 컴포넌트 기능 일부 개선

- 설치 후 resolutions에 아래 내용 추가 필요함.

```json
"resolutions": {
  "highlight.js": "10.6.0",
  "postcss-loader": "3.0.0",
  "sass": "1.32.12"
},
```

## **2.0.3-stable (2021/6/2)**

시스템 공통 기능 적용

## **2.0.2-stable (2021/6/1)**

시스템 공통 기능 안정화 버전

Static 실시간 프로파일 추출 및 보안 요소 추가

## **2.0.1-stable**

최초 Release


# Release Note (Nexacro)
## 1.0.3 (2021/10/07)

그리드 연계 기능 추가

Axios 통신 라이브러리 업데이트

팝업 표준화

입력 샘플 추가

## 1.0.2 (2021/09/15)

로그인 연계 기능 추가

메뉴 관리 기능 추가

## 1.0.1 (2021/09/13)

팝업 연계 기능 추가

그리드 페이징 연계 기능 추가

Variable 파라메터 Object, Generic Type 매핑 기능 추가


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
