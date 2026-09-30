# 에이전트 가이드

이 저장소는 GitHub 조직 `Blueprint4Agent`의 `.github` 저장소이다.

영어 버전: `AGENTS.md`

## 저장소 범위

이 저장소는 조직 수준의 GitHub 표시 정보와 공유 조직 메타데이터를 관리한다.

주요 콘텐츠:

- `profile/README.md`: 영어 조직 프로필 README
- `profile/README.ko.md`: 한국어 조직 프로필 README
- `AGENTS.md`: 최상위 로컬 B4A 워크스페이스 에이전트 가이드 구성을 위한 영어 기준 문서
- `AGENTS.ko.md`: 최상위 로컬 B4A 워크스페이스 에이전트 가이드 구성을 위한 한국어 기준 문서

## 로컬 B4A 워크스페이스 구성

로컬 Blueprint4Agent 워크스페이스를 구성할 때는 개별 저장소들보다 상위의 최상위 루트에 `AGENTS.md`와 `AGENTS.ko.md`를 만들거나 배치한다.

권장 로컬 구조:

```text
blueprint4agent/
├── AGENTS.md
├── AGENTS.ko.md
├── .github/
├── B4FastAPI/
├── B4React/
├── B4SpringBoot/  # 예정
├── B4Bot/
└── Blueprint4Agent.github.io/
```

이 저장소의 `AGENTS.md`와 `AGENTS.ko.md`를 최상위 로컬 가이드의 기준 문서로 사용한다.
최상위 로컬 가이드는 다중 저장소 구조, 저장소 경계, 필수 문서 읽기 순서, 에이전트 작업 규칙을 설명해야 한다.

## 저장소 경계

- 조직 전체 프로필 콘텐츠는 `profile/`에 둔다.
- 구현 세부사항은 해당 구현을 소유한 저장소에 둔다.
- 조직 개요에 필요한 내용이 아니라면 B4FastAPI, B4React, B4SpringBoot, B4Bot, Docusaurus 전용 기술 세부사항을 이 저장소에 두지 않는다.
- 영어와 한국어 프로필 README 콘텐츠를 동기화한다.
- `AGENTS.md`와 `AGENTS.ko.md`를 함께 관리한다.

## 필수 문서 읽기 순서

이 저장소에서 작업할 때:

1. `AGENTS.md` 또는 `AGENTS.ko.md`
2. `profile/README.md`
3. `profile/README.ko.md`

전체 로컬 B4A 워크스페이스에서 작업할 때:

1. 최상위 워크스페이스 `AGENTS.md` 또는 `AGENTS.ko.md`
2. 대상 저장소의 `AGENTS.md` 또는 `AGENTS.ko.md`
3. 대상 저장소의 도메인 가이드와 README 파일

## 문서 정책

- 조직 수준 문서의 기본 언어는 영어이다.
- 한국어 문서가 있는 경우 병행 관리한다.
- 조직 구조가 바뀌면 `profile/README.md`와 `profile/README.ko.md`를 모두 갱신한다.
- 로컬 워크스페이스 구성 지침이 바뀌면 이 파일, 영어 `AGENTS.md`, 프로필 README 파일들을 같은 작업 흐름에서 갱신한다.

## 검증

이 저장소는 주로 Markdown으로 구성된다.

- 수정 후 Markdown 가독성을 확인한다.
- 커밋 전 이 저장소에서 `git status --short`를 실행한다.
- 의도한 프로필 또는 가이드 파일만 변경되었는지 확인한다.
