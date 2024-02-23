# U.STRA Framework

GSITM에서 운영 중인 U.STRA Framework 공식 Release Repository 입니다.

## 공식 가이드 안내

공식 가이드 사이트 : http://guide.ustraframework.kro.kr/

현재 공식 가이드는 일부 기능을 제한적으로 운영 중에 있습니다. 다음 기능이 제한됩니다.

- 데모 서비스
- 공지사항

문의 사항은 [이슈](https://github.com/ustraframework/ustraframework/issues)로 등록해 주시기 바랍니다.


## 공식 의존성 저장소 변경 안내

GSITM 전사 자원 정책 변경으로 의존성 저장소를 변경할 예정입니다.

현재는 임시 저장소를 제공하고 있으니 참고하기 바랍니다.

- 메이븐 레파지토리 : http://repo.ustraframework.kro.kr/repository/maven-public/
- NPM 레지스트리 : http://repo.ustraframework.kro.kr/repository/npm-public/


## Release Note (Java)

### 2.0.41 RELEASE (**2021/10/6**)

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
