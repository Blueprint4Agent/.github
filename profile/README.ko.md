# Blueprint4Agent

Blueprint4Agent는 **에이전틱 코딩(Agentic Coding)을 위한 웹 서버 블루프린트(템플릿) 조직**입니다.
실무에서 바로 사용할 수 있도록 **de facto 우선** 기준으로 설계하며, 에이전틱 자동화 워크플로우에 최적화된 구성을 제공합니다.

현재는 **FastAPI 기반 모놀리식 블루프린트**를 제공하고 있으며,
추후 **Node.js**, **Spring Boot** 등 다양한 웹 서버 프레임워크 블루프린트를 추가할 예정입니다.

궁극적으로는 이 조직 구조를 그대로 활용해, 각 팀이 GitHub 프로젝트를 **에이전틱 코딩 방식으로 즉시 시작하고 운영**할 수 있도록 하는 것이 목표입니다.

## 목표

- GitHub Pages + Docusaurus 기반 문서 웹사이트 제공
- 스펙 문서, 매뉴얼, 프로젝트 문서를 위한 기본 템플릿 제공
- 에이전트 자동화 봇 기반 프로젝트 자동 검토 및 이슈 생성 플로우 제공

## 저장소 구조

```text
Blueprint4Agent/
├── AGENTS.md
│   └── 여러 저장소로 구성된 B4A 로컬 워크스페이스를 관리하는 최상위 영어 에이전트 가이드
├── AGENTS.ko.md
│   └── 여러 저장소로 구성된 B4A 로컬 워크스페이스를 관리하는 최상위 한국어 에이전트 가이드
├── .github
│   ├── AGENTS.md
│   ├── AGENTS.ko.md
│   └── 조직 프로필, 공통 정책, 워크플로우 템플릿
├── Blueprint4Agent.github.io
│   └── Docusaurus 기반 프로젝트 문서 웹사이트 (GitHub Pages)
├── B4FastAPI
│   └── FastAPI 기반 웹 서버 블루프린트 (현재 모놀리식)
└── B4Bot
    └── 에이전트 기반 프로젝트 관리 봇 및 scope별 이슈 생성 액션
```

B4A 로컬 워크스페이스를 구성할 때는 개별 저장소들보다 상위의 최상위 루트에 `AGENTS.md`와 `AGENTS.ko.md`를 배치합니다.
이 파일들을 여러 저장소 구조, 저장소 경계, 필수 문서 읽기 순서, 에이전트 작업 규칙을 조율하는 루트 가이드로 사용합니다.

`.github` 저장소는 저장소 루트에 `AGENTS.md`와 `AGENTS.ko.md`를 포함하며, 이 파일들을 로컬 구성의 기준 문서로 사용합니다.
실제 사용 시에는 개별 저장소 내부에만 두지 말고, 로컬 워크스페이스 최상위 루트에 이 가이드들을 구성합니다.

## 방향성

Blueprint4Agent는 단순 코드 템플릿 조직이 아니라,
코드, 문서, 자동화, 검토 워크플로우를 아우르는 **에이전틱 개발 기반(agentic development foundation)** 제공을 지향합니다.

---

English version: [README.md](./README.md)
