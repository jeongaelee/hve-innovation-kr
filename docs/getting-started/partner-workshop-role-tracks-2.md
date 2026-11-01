---
title: 파트너 워크샵 - 역할별 트랙 Part2- PM 및 기술 트랙
description: HVE 파트너 워크샵을 위한 프로젝트 관리 및 기술 역할 가이드
sidebar_position: 10
author: Microsoft
ms.date: 2026-11-01
ms.topic: tutorial
keywords:
  - Project Manager
  - System Architecture Reviewer
  - Security Planner
  - HVE technical track
estimated_reading_time: 10
---

## 워크샵 일정

| 단계 | 활동                                                                                       | 시간   |
|------|-------------------------------------------------------------------------------------------|-------|
| 1    | [워크샵 개요](partner-workshop.md)                                                     | 30분 |
| 2    | [**로컬 VS Code 설정**](partner-workshop-setup.md)                                            | 30분 |
| 3-1    | [역할별 트랙 Part1: 계획/비전/경험](partner-workshop-role-tracks.md)                      | 45분 |
| 3-2    | [역할별 트랙 Part2: 아키텍처 설계, 백로그](partner-workshop-role-tracks-2.md)                 | 45분 |
| 4    | [검증 및 솔루션](partner-workshop-solution.md)                                             | 30분 |
| 5    | [Microsoft Marketplace 및 Copilot Agent Store 준비](partner-workshop-publishing.md)       | 60분 |
| 6    | [구현 및 상용화로의 핸드오프](partner-workshop-implementation.md)                            | 30분 |

이 문서는 파트너 워크샵의 프로젝트 관리 및 기술 트랙을 다룹니다. 요구사항, 사용자 경험,
구현 계획을 검토한 뒤 솔루션 접근 방식, 아키텍처, 보안 및 게시 고려
사항을 구성하세요.

## 프로젝트 관리 (PM) 트랙

### 목표

비즈니스 컨텍스트와 사용자 경험을 요구사항, 우선순위, 구현 계획을 갖춘
백로그 초안으로 전환하세요.

### 단계

1. `.copilot-tracking/research/`, `.copilot-tracking/prd-sessions/`,
   `.copilot-tracking/brd-sessions/`, `.copilot-tracking/dt/`의
   컨텍스트 패키지를 검토하세요. 이를 비즈니스 결과, 측정 가능한 성공
   지표, 기능 및 비기능 요구사항, 사용자 스토리, 수락 기준, 범위 외
   항목, 미해결 가정과 정렬하세요.
2. **RPI Agent**를 선택하고 `/rpi-plan`을 실행하여 요구사항과
   컨텍스트를 단계와 단계별 세부 사항을 갖춘 구현 계획으로
   전환하세요. 예시:

   ```text
   /rpi-plan Read `.copilot-tracking/research/,
   `.copilot-tracking/brd-sessions/` and `.copilot-tracking/dt/`. Create a
   lightweight implementation plan for the first MVP of the [Relationship
   Manager
   Assistant for FSI]. Include phase objectives, deliverables, requirements,
   dependencies, risks, and acceptance criteria. Plan for one evidence-backed
   job
   with grounded responses, source citations, permission-aware retrieval, clear
   uncertainty, human escalation, and confirmation before external actions.
   Align the plan to Microsoft Marketplace and Microsoft 365 Copilot Agent Store
   readiness, but keep publication claims provisional until current Microsoft
   guidance, Partner Center state, and tenant feasibility are verified. Do not
   implement or publish anything.
   ```

   이는 `.copilot-tracking/plans/`에 작성되며 요구사항과 디자인
   컨텍스트에 연결되는 영구 기록을 만듭니다.

3. `.copilot-tracking/plans/`에 생성된 계획을 검토하고 필요에 따라
   단계별 세부 사항을 다듬으세요.
4. 팀이 요구사항에서 구현으로 이동하는 데 도움이 될 때만 백로그
   개요를 만드세요. 필요하다면 첫 MVP를 위해 에픽, 기능, 스토리, 작업과
   같은 가벼운 계층 구조를 사용하세요.
5. 팀에 순서 신호가 필요한 경우에만 P0, P1, P2와 같은 간단한 레이블로
   첫 MVP의 우선순위를 지정하세요. 이를 경직된 Agile 프로세스로
   만들기보다는 가볍고 결과 중심으로 유지하세요.
6. Microsoft Marketplace와 Microsoft 365 Copilot Agent Store의 게시
   준비를 위해 요구사항과 백로그 아티팩트를 준비하세요.
   컨텍스트, 요구사항, 경험을 선택하고 **Functional Planner**에게
   프롬프트하세요:

```text
"Use the functional-planner skill and review the requirements under
`.copilot-tracking/prd-sessions/`, the context under
`.copilot-tracking/research/`, and the experience draft under
`.copilot-tracking/dt/`. Create or refine a more implementation-ready MVP
backlog
plan under `.copilot-tracking/github-issues/` with clear epics, features,
stories,
and tasks. Then prioritize the MVP with simple labels such as P0, P1, and P2
only
if they help sequence the work. Also assess publication readiness for Microsoft
Marketplace and Microsoft 365 Copilot Agent Store. Keep the output concise,
outcome-focused, and useful for backlog refinement."
```

1. GitHub Issues를 대상으로 한다면 Backlog Manager에게 워크플로우를
   조율하도록 요청하고 GitHub Backlog Executor가 초기 MVP를 위한 첫
   상위 이슈와 하위 이슈를 생성하도록 하세요. **Backlog Manager**는
   추적성을 위해 결과로 생성된 이슈 링크와 요약을
   `.copilot-tracking/github-issues/` 아래에 기록되도록 해야 합니다.

   GitHub 이슈 작성 활성화:

   * GitHub CLI 인증
     * 실행: gh auth login --web
     * 또는 필요하다면: gh auth refresh -h github.com -s repo
   * 인증 확인
     * 실행: gh auth status
   * 대상 저장소 확인
     * 실행: gh repo set-default [your git clone url]/hve-partner-workshop
   * GitHub 쓰기 도구가 노출된 세션에서 백로그 생성을 통해 GitHub
     Issues 생성
     * Copilot이나 에이전트 워크플로우를 사용한다면 세션이 GitHub MCP
       쓰기 도구에 접근할 수 있는지 확인하세요.
     * [Copilot Chat에서 GitHub MCP 서버 사용하기](https://docs.github.com/en/copilot/how-tos/copilot-on-github/copilot-for-github-tasks/using-the-github-mcp-server-from-copilot-chat)를
       참고하세요.
     * [IDE에서 GitHub MCP 서버 사용하기](https://docs.github.com/en/copilot/how-tos/provide-context/use-mcp-in-your-ide/use-the-github-mcp-server)를
       참고하세요.

   프롬프트:

```text
"Review the approved requirements under `.copilot-tracking/prd-sessions/` and
the
backlog outline under `.copilot-tracking/github-issues/`. Confirm the target
GitHub repository, create the first parent issue and child issues for this
initial MVP, and record the issue links and summary under
`.copilot-tracking/github-issues/` for traceability. Use labels such as P0, P1,
P2, epic, feature, story, and task only if they help the workflow. Update the
backlog plan and create the backlog in GitHub Issues."
```

1. 비즈니스 결과에서 요구사항, 백로그 항목까지의 추적성을 위해 이슈
   목록을 검토한 후, 최종 백로그 요약과 이슈 링크를
   `.copilot-tracking/github-issues/` 아래에 저장하세요.

### 결과물

1. **구현 계획**(`.copilot-tracking/plans/`): 각 단계의 목표,
   결과물, 수락 기준을 갖춘 단계별 구현 계획.
2. **GitHub 백로그**(`.copilot-tracking/github-issues/`): 비즈니스
   결과를 추적 가능한 작업 항목으로 전환하기 위한 기능, 스토리, 작업의
   백로그로, 구현 계획에 연결되어 있습니다.

## 기술 트랙

### 목표

구현 계획에 맞춰 솔루션 접근 방식, 아키텍처, 게시 고려 사항을
구성하세요.

### 단계

1. `.copilot-tracking/brd-sessions/`, `copilot-tracking/prd-sessions/`
   아래의 요구사항, `.copilot-tracking/dt/` 아래의 경험 초안,
   `.copilot-tracking/plans/`의 구현 계획을 검토하세요.
2. 단계별 계획을 뒷받침하는 핵심 서비스, 데이터 소스, 통합 지점을
   식별하세요.
3. 계획의 각 단계와 정렬되는 간단한 솔루션 접근 방식, 주요
   트레이드오프, 아키텍처 노트를 구성하기 위해
   **System Architecture Reviewer**를 선택하세요:

   * 배포, 보안, 운영 고려 사항을 기록하세요.
   * Well-Architected 설계와 Cloud Adoption Framework 가이드에
     비추어 초안을 검토하세요.
   * 패키징, 발견 가능성, 지원 가능성, 통합 기대치를 포함하여
     Microsoft Marketplace와 Microsoft 365 Copilot Agent Store 준비를
     위한 게시 요구사항을 포착하세요.

   ```text
   "Review the implementation plan at `.copilot-tracking/plans/`, the
   requirements
   under `.copilot-tracking/prd-sessions/`, and the experience draft under
   `.copilot-tracking/dt/`. Create architecture notes under
   `.copilot-tracking/details/` covering a simple solution approach for each
   phase, major tradeoffs, cloud architecture, well-architected concerns,
   publication requirements, Microsoft IQ, and a Mermaid architecture diagram.
   Link the architecture notes back to the phases in the implementation plan."
   ```
   * **Arch Diagram Builder**를 선택하여 간단한 Mermaid 아키텍처
     다이어그램을 만드세요.

4. 각 단계에 맞춰 준비 상태를 검토하고 후속 작업을 드러내기 위해
   **Security Planner**를 사용하세요.

   ```text
   "Review this solution draft for security risks, deployment considerations,
   and
   follow-up actions needed for each phase in the implementation plan. Link any
   security-related work back to the appropriate phase."
   ```

5. Mermaid 다이어그램을 검토하고 자연어로 다듬으세요.
6. (선택 사항) GitHub Copilot 대신 **Microsoft 365 Copilot**을 사용하여
   이미지를 만드세요. M365 Copilot에서 구현 계획을 첨부하고, Azure와
   Copilot 스타일 아이콘을 사용해 첫 MVP의 핵심 서비스, 데이터 소스,
   사용자 경험 계층, 통합을 나타내는 아키텍처 이미지를 Mermaid
   다이어그램에서 만드세요.

   ```text
   "Create an architecture image from the Mermaid diagram for this solution
   using
   Azure and Copilot-style icons to represent core services, data sources, user
   experience layers, and integrations for the first MVP. "
   ```
   검토된 이미지를 `.copilot-tracking/details/` 아래에 저장하거나
   참조하세요.

7. 솔루션 검토에 필요한 게시 가정만 아키텍처 노트에 포착하고 구현
   계획에 링크하세요.

   * SaaS 또는 Azure Managed Application을 선호하는 Marketplace
     모델로 선택하고 Microsoft 365 에이전트를 잠재적인 컴패니언
     경험으로 선택하세요.
   * Managed Application: 구성 요소가 무엇을 배포하는지, 에이전트가
     사용자에게 무엇을 보여주는지, 각 제품 경계가 어디서 시작되고
     끝나는지 명시하세요.
   * 두 제품 간 API, 아이덴티티, 권한, 데이터 계약을 요약하세요.
   * 데이터 상주, 테넌트 격리, 고객 통제 인프라, 최소 권한 접근을
     포함하여 솔루션에 영향을 미치는 아키텍처 제약을 기록하세요.
   * 담당자와 함께 미해결 게시 가정을 나열하세요. 역할 실습 중에
     상업적 또는 제출 세부 사항을 해결하지 마세요.

   **RPI Agent**를 선택하세요.

   ```text
   "Review the implementation plan at `.copilot-tracking/plans/`, the
   requirements
   under `.copilot-tracking/prd-sessions/`, the experience draft under
   `.copilot-tracking/dt/`, and the architecture notes under
   `.copilot-tracking/details/`. Update the architecture notes with only the
   publication assumptions needed for the solution review. Record preferred
   Marketplace model and the Microsoft 365 agent as a potential companion
   experience. Define the product boundaries and summarize the API, identity,
   permission, and data contract between them. Capture only architecture
   constraints, assumptions, unresolved decisions, and owners needed for
   solution
   integration. Link these inputs to the implementation plan. Defer the
   Marketplace implementation plan, offer validation, pricing, monetization,
   Partner Center configuration, package preparation, certification, and rollout
   planning to the Partner Workshop Publishing Follow-Up."
   ```

   [파트너 워크샵 게시 후속 작업](partner-workshop-publishing)에서 상세한
   준비 상태 평가를 완료하세요.

8. 나머지 팀과 결과를 공유하세요.

### 결과물

1. **아키텍처 노트**(`.copilot-tracking/details/`): 위험, 트레이드오프,
   통합 요구사항, 솔루션 검토에 필요한 최소한의 게시 가정을 포함하여
   구현 계획의 각 단계에 맞춘 아키텍처 설계 노트.
2. 게시 계획 입력: 잠정적인 제품 분할, 통합 경계, 아키텍처 제약,
   게시 워크샵을 위해 아키텍처 노트 안에 기록된 미해결 결정 사항.

## 작업 세션 알림

결과물을 간결하고 실행 지향적으로 유지하세요. 완벽한 정보를 기다리지
마세요. 목표는 팀이 워크샵 이후 다듬을 수 있는 검토된 초안을 만드는
것입니다.

## 다음 단계
[**검증 및 솔루션**](partner-workshop-solution.md)을 진행하세요.

---

<!-- markdownlint-disable MD036 -->
*🤖 Crafted with precision by ✨Copilot following brilliant human instruction,
then carefully refined by our team of discerning human reviewers.*
<!-- markdownlint-enable MD036 -->
