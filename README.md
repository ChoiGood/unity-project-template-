# Unity Project GitHub Template

이 저장소는  
**소규모 Unity 게임 팀을 가정한 Git & CI 템플릿 리포지토리**입니다.

혼자 하는 프로젝트라도  
실제 게임 개발 환경에 가까운 방식으로  
브랜치 전략, CI, 협업 규칙을 연습하는 것을 목표로 합니다.

---

## 🎯 목표

- Unity 프로젝트에 적합한 Git 전략 정리
- main 브랜치 안정성 유지
- 빌드 실패를 조기에 발견
- “혼자서도 팀처럼 개발하기”

---

## 🌿 브랜치 전략

GitHub-flow 변형 구조를 사용합니다.

main
└─ feature/*


### 규칙

- `main` 브랜치는 항상 실행 가능한 상태 유지
- 직접 커밋 금지
- 모든 작업은 `feature/*` 브랜치에서 진행
- Pull Request + CI 통과 후 병합

---

## 🔁 작업 흐름

1. `feature/*` 브랜치 생성
2. 기능 개발
3. Pull Request 생성
4. CI 빌드 통과 확인
5. `main` 브랜치로 병합

> ⚠️ merge = deploy ❌  
> ✔️ merge = 안정 상태 유지

---

## 🤖 CI 정책

- Unity 프로젝트 빌드 자동화
- 컴파일 에러 및 빌드 실패 사전 방지
- 배포 및 스토어 업로드는 자동화하지 않음

CI는 **검증 도구**이며  
출시를 대신하지 않습니다.

---

## 🚫 Git Ignore

Unity 프로젝트 특성상  
다음 폴더는 Git에 포함하지 않습니다.

- Library
- Temp
- Obj
- Build / Builds
- Logs

---

## Git Commit Convention

- feat: 기능 추가
- fix: 버그 수정
- asset: 에셋 변경
- prefab: 프리팹 수정
- scene: 씬 변경
- anim: 애니메이션 작업
- ui: UI 작업
- balance: 밸런스 조정
- refactor: 구조 개선
- chore: 환경 설정

## 🔍 Pull Request

- 모든 변경 사항은 Pull Request를 통해 병합합니다.
- PR 작성 시 템플릿을 기준으로 변경 내용과 빌드 상태를 확인합니다.

---


## 📌 이 템플릿이 의미하는 것

이 저장소는 단순한 코드 저장소가 아니라,

- Git 전략에 대한 이해
- Unity 프로젝트 구조 이해
- 게임 개발에서 CI의 역할에 대한 판단
- 소규모 팀 개발 현실에 대한 인식

을 함께 보여주기 위한 템플릿입니다.