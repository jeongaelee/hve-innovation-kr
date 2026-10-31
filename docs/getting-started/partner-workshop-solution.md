---
title: 파트너 워크숍 솔루션
description: 역할별 결과물을 공유 솔루션 패키지, 백로그, 아키텍처 뷰, 게시 준비 계획으로 통합
sidebar_position: 10
author: Microsoft
ms.date: 2026-10-31
ms.topic: tutorial
keywords:
  - workshop solution
  - backlog
  - requirements traceability
  - Azure diagram
  - publication readiness
estimated_reading_time: 8
---

## 워크숍 일정

| 단계 | 활동                                                                                       | 시간   |
|------|---------------------------------------------------------------------------------------------|--------|
| 1    | [워크숍 개요](partner-workshop.md)                                                           | 30분 |
| 2    | [Codespaces 또는 로컬 VS Code 설정](partner-workshop-setup.md)                               | 30분 |
| 3    | [계획, 비전, 경험, 아키텍처 설계, 백로그](partner-workshop-role-tracks.md)                    | 90분 |
| 4    | [**검증 및 솔루션**](partner-workshop-solution.md)                                            | 30분 |
| 5    | [Microsoft Marketplace 및 Copilot Agent Store 준비](partner-workshop-publishing.md)          | 60분 |
| 6    | [구현 및 상용화로의 핸드오프](partner-workshop-implementation.md)                             | 30분 |

워크숍의 솔루션 단계에서 이 가이드를 사용하세요. 참가자는 역할별 결과물을
한데 모으고, 공백과 추적성을 확인하며, 세션 이후에도 다듬을 수 있는 검토된
핸드오프를 남겨야 합니다.

## 목표

비즈니스 컨텍스트, 요구사항, 경험, 백로그, 아키텍처, 게시 준비 상태를 하나의
일관된 이야기로 연결하는 공유 솔루션 초안을 만드세요.

## 권장 솔루션 흐름

1. 각 역할에게 2분 동안 자신의 아티팩트를 요약하도록 요청하세요.
2. `.copilot-tracking/research/`, `.copilot-tracking/prd-sessions/`,
   `.copilot-tracking/dt/`, `.copilot-tracking/plans/`,
   `.copilot-tracking/details/`, `.copilot-tracking/github-issues/` 아래의
   프로덕션 아티팩트를 여세요.
3. 파일 간 용어를 비교하고 모순을 해결하세요.
4. SME 컨텍스트 패키지를 도메인 용어와 비즈니스 규칙의 신뢰할 수 있는
   소스로 사용하세요.
5. 각 사용자 스토리가 사용자, 필요, 결과를 식별하는지 확인하세요.
6. 각 수락 기준이 관찰 가능하고 테스트 가능한지 확인하세요.
7. 각 아키텍처 구성 요소가 최소 하나의 요구사항에 매핑되는지 확인하세요.
8. 고위험 요구사항과 중요한 결정이 백로그 항목에 매핑되는지 확인하세요.
9. 경험이 불확실성, 피드백, 접근 실패, 사람의 개입(에스컬레이션)을
   포착하는지 확인하세요.
10. 게시 워크숍을 위해 미해결 게시 입력을 아키텍처 노트에 기록하세요.

## 추적성 검토

**RPI-Plan**을 선택하고 다음 프롬프트를 입력하세요:

```text
"Review the production artifact set under `.copilot-tracking/research/`,
`.copilot-tracking/prd-sessions/`, `.copilot-tracking/dt/`,
`.copilot-tracking/plans/`, `.copilot-tracking/details/`, and
`.copilot-tracking/github-issues/` as one solution pack. Build a traceability
matrix from context facts and decisions to requirements, experience needs,
architecture components, backlog items, tests, and publication gates. Save
the matrix under `.copilot-tracking/details/`. Report missing links,
contradictions, unsupported claims, and unowned risks. Do not implement or
publish anything."
```

그런 다음 다음 단계를 완료하세요:

1. `.copilot-tracking/details/` 아래에 매트릭스 초안을 기록하세요.
2. 각 공백에 담당자를 지정하세요.
3. 워크숍 증거로 해결할 수 있는 공백을 수정하세요.
4. 담당자와 함께 남은 게시 공백을 아키텍처 노트에 기록하세요.
5. 책임 있는 사람이 검토할 때까지 생성된 콘텐츠를 초안으로 표시하세요.

다음 워크숍에서는 이러한 게시 입력을 Microsoft Marketplace Coach에
전달하며, 이 Coach는 `.copilot-tracking/plans/` 아래에 정식 Marketplace
구현 계획을 만듭니다. 솔루션 검토 중에는 별도의 게시 준비 아티팩트를 만들지
마세요.

### 프로젝트 매니저: GitHub Issues

1. **Backlog Manager**를 선택하세요.
2. `.copilot-tracking/github-issues/` 아래의 백로그 계획을 준비 상태와
   중복 여부를 기준으로 검사하도록 요청하세요.
3. 저장소, 레이블, 마일스톤, 담당자, 이슈 계층 구조를 확인하세요.
4. 변경 전에 드라이런(dry-run) 요약을 요청하세요.
5. 제안된 이슈 제목과 수락 기준을 검토하세요.
6. 퍼실리테이터의 승인과 저장소 권한이 있을 때만 이슈를 생성하세요.

### 프로젝트 매니저: Markdown 전용 대안

1. `.copilot-tracking/github-issues/` 아래의 백로그 계획을
   시스템 중립적인 백로그로 유지하세요.
2. 대상 시스템, 담당자, 상태, 외부 ID를 위한 열을 추가하세요.
3. 승인된 각 항목을 워크숍 이후에 가져오거나 생성할 담당자를 지정하세요.

### 엔지니어: 아키텍처 검토

1. `.copilot-tracking/details/`에 있는 아키텍처 노트와 다이어그램을
   Markdown 미리보기로 여세요.
2. Microsoft 365 Copilot에서의 주요 사용자 요청을 Azure API, 검색 계층,
   모델, 응답 경로까지 따라가세요.
3. 콘텐츠 수집 및 업데이트 경로를 별도로 따라가세요.
4. 권한 부여가 어디에서 적용되는지 식별하세요.
5. 비밀 정보와 키가 어디에 저장되는지 식별하세요.
6. 프롬프트, 검색된 콘텐츠, 응답, 피드백이 어디에서 기록될 수 있는지
   식별하세요.
7. 텔레메트리가 비밀 정보나 불필요한 개인 데이터를 수집하지 않는지
   확인하세요.
8. 모델, 검색, 아이덴티티, 종속성 장애에 대한 실패 경로를 추가하세요.
9. 비용 담당자와 운영 담당자를 추가하세요.
10. 인프라 소스와 배포 검증이 존재할 때까지 다이어그램을 개념적인 것으로
    표시하세요.

## 10분 팀 토론

1. PM이 결과, 요구사항, 첫 출시 범위를 발표합니다.
2. SME가 주요 제약과 미해결된 도메인 질문을 발표합니다.
3. 디자이너가 주요 여정과 사람의 검토 지점을 발표합니다.
4. 기술 리드가 아키텍처 뷰와 게시 경로를 발표합니다.
5. 팀이 가장 큰 위험 세 가지를 지목합니다.
6. 퍼실리테이터가 담당자와 다음 검토 일정을 확인합니다.

[게시 가이드](partner-workshop-publishing.md)로 진행하세요.

---

<!-- markdownlint-disable MD036 -->
*🤖 Crafted with precision by ✨Copilot following brilliant human instruction,
then carefully refined by our team of discerning human reviewers.*
<!-- markdownlint-enable MD036 -->
