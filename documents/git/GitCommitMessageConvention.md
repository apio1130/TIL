# Angular Git Commit Message Convention
각 커밋 메시지는 머리글(hader)과 본문(body), 바닥글(footer) 로 구성.

```
<header>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```
- header: 필수이며 커밋 메시지 헤더 방식으 따라야 함
- body: dosc tpye 을 제외한 모든 커밋에 필수로 커밋 메시지 본문 형식을 따라야 함
- footer: 선택사항으로 용도와 footer 의 구조를 설명

## 커밋 메시지 헤더
```
<type>(<scope>): <short summary>
  │       │             │
  │       │             └─⫸ Summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Commit Scope: animations|bazel|benchpress|common|compiler|compiler-cli|core|
  │                          elements|forms|http|language-service|localize|platform-browser|
  │                          platform-browser-dynamic|platform-server|router|service-worker|
  │                          upgrade|zone.js|packaging|changelog|docs-infra|migrations|ngcc|ve|
  │                          devtools
  │
  └─⫸ Commit Type: build|ci|docs|feat|fix|perf|refactor|test
```

### Type
- feat: 새 기능
- fix: 버그 수정
- dosc: 문서만 변경
- style: 코드의 의미에 영향을 미치지 않는 변경 사항(공백, 포맷팅, etc)
- refactor: 버그를 수정하거나 기능을 추가하지 않는 코드 변경(bug fix가 아닌 수정과 사용하지 않는 코드 삭제 등)
- perf: 성능을 향상시키는 코드 변경
- test: 누락된 테스트 추가 또는 기존 테스트 수정
- build: 빌드 시스템 또는 외부 종속성에 영향을 주는 변경 사항(예시 scopes : gulp, broccoli, npm 등)
- ci: CI 구성 파일 및 스크립트 변경(예시 scopes : Travis, Circle, SauceLabs 등)
- chore: src 또는 테스트 파일을 수정하지 않는 기타 변경 사항
- revert: 이전 커밋을 되돌림

### scope
영향을 받는 npm 패키지의 이름.

### short summary
변경 사항에 대한 간결한 설명을 제공.
- 명령형, 현재 시제 사용
- 첫 글자를 대문자로 사용 금지
- 끝에 점(.) 없음

## 커밋 메시지 본문
커밋 메시지 본문을 변경한 동기를 설명.
- 명령형 현재 시제를 사용
- 이 커밋 메시지는 변경 이유를 설명해야 합
- 변경의 영향을 설명하기 위해 새 동작과 이전 동작의 비교를 포함할 수 있음

## 커밋 메시지 바닥글
주요 변경 사항 및 사용 중단에 대한 정보가 포함될 수 있으며 GitHub 문제, Jira 티켓 및 이 커밋이 종료되거나 관련된 기타 PR을 참조할 수도 있음.

## 참고
- https://github.com/angular/angular/blob/main/CONTRIBUTING.md
