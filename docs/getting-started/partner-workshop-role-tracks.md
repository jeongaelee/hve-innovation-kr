---
title: 파트너 워크샵 - 역할별 트랙 Part1- 계획/비전/경험
description: HVE 파트너 워크샵을 위한 구조화된 역할 기반 가이드
sidebar_position: 9
author: Microsoft
ms.date: 2026-10-31
ms.topic: tutorial
keywords:
  - Project Manager
  - Subject Matter Expert
  - UX Designer
  - Engineer
  - HVE roles
estimated_reading_time: 10
---

## 워크샵 일정

| 단계 | 활동                                                                                       | 시간   |
|------|-------------------------------------------------------------------------------------------|-------|
| 1    | [워크샵 개요](partner-workshop.md)                                                     | 30분 |
| 2    | [로컬 VS Code 설정](partner-workshop-setup.md)                                            | 30분 |
| 3    | [**역할별 트랙 Part1: 계획/비전/경험**](partner-workshop-role-tracks.md)                      | 45분 |
| 3    | [역할별 트랙 Part2: 아키텍처 설계, 백로그](partner-workshop-role-tracks-2.md)                 | 45분 |
| 4    | [검증 및 솔루션](partner-workshop-solution.md)                                             | 30분 |
| 5    | [Microsoft Marketplace 및 Copilot Agent Store 준비](partner-workshop-publishing.md)       | 60분 |
| 6    | [구현 및 상용화로의 핸드오프](partner-workshop-implementation.md)                            | 30분 |

## 권장 역할 순서

워크숍은 다음과 같은 순서로 진행하는 것이 효과적입니다.:

1. 주제 전문가(SME)가 팀이 함께 사용할 공통 컨텍스트를 만듭니다.
2. 프로젝트 관리(PM)가 초안을 요구사항, 우선순위, 백로그 구조로 전환합니다.
3. 디자인(Design)이 해당 컨텍스트를 사용자 경험 초안으로 전환하고, 접근성과 책임 있는 AI 요구사항을 정의합니다.
4. 기술(Technical)이 솔루션 접근 방식, 아키텍처, 게시(Publication) 관련 고려 사항을 구체화합니다.
5. 마지막으로, 솔루션 통합 단계에서 팀 전체가 각 역할의 결과문과 인계(Handoff) 내용을 함께 검토합니다.

이 순서는 각 역할이 완벽한 정보를 기다리지 않고도 이전 역할의 결과물 위에 구축할 수 있도록 돕습니다.

## HVE 대 Agile

| Agile                                            | HVE                                                       |
|---------------------------------------------------|-------------------------------------------------------------|
| 스프린트 우선, 기능 우선                           | 결과 우선, 가치 우선                                         |
| 백로그 구체화가 전달을 주도하는 경우가 많음           | 공유된 컨텍스트와 AI 기반 계획이 딜리버리를 주도함                 |
| 팀이 요구사항을 서로 다르게 해석하는 경우가 많음    | 사람과 에이전트가 동일한 컨텍스트와 근거를 바탕으로 함께 작업           |
| 많은 기능을 너무 이른 단계부터 검토하게 될 수 있음     | 작은 단위의 결과에 집중하면 팀이 빠르게 학습할 수 있음        |

## 트랙 개요

| 트랙             | 핵심 목표                                                  | 권장 결과물                             |
|-------------------|-------------------------------------------------------------|-------------------------------------------|
| 프로젝트 관리     | 컨텍스트를 요구사항, 우선순위, 백로그 구조로 전환            | 요구사항 초안과 백로그 개요             |
| 주제 전문가(SME)  | 비즈니스 사실, 규칙, 제약, 증거 수집                          | 컨텍스트 패키지                         |
| 디자인            | 사용자 경험, 어려움, 성공 기준 표현                          | 경험 초안                               |
| 기술              | 솔루션, 아키텍처, 배포 고려 사항 구성                         | 아키텍처 및 게시 노트                   |

## HVE 에이전트 가이드

HVE 에이전트를 역할을 위한 가벼운 도우미로 사용하세요. 자신의 초안부터시작한 후 에이전트에게 다듬거나 구조화하도록 요청하세요.

* 비즈니스 결과, 범위, 수락 기준을 위한 첫 초안 요구사항과 간단한 구조를 위해 **BRD Builder** 또는 **PRD Builder**를 사용하세요. 이 워크샵에서는 일반적으로 프로젝트 관리 역할이 BRD/PRD 초안을 소유하고, SME는 그 근거가 되는 비즈니스 컨텍스트, 증거, 제약을 제공합니다.
* SME가 공유 컨텍스트 패키지를 만들기 전에 증거를 수집, 테스트, 종합하기 위해 **RPI Agent**를 사용하세요.
* 팀이 전달 핸드오프가 필요할 때, 초안 요구사항을 가벼운 에픽, 기능, 스토리, 작업 계층 구조로 전환하기 위해 **Functional Planner**를 사용하세요.
* 사용자 여정, 어려움, 와이어프레임 개요, 경험 아티팩트를 위해 **UX UI Designer**를 사용하세요.
* 퍼실리테이션과 디스커버리를 위해 **Design Thinking Coach**를 사용하세요.
* 안내된 학습과 방법 지원을 위해 **Design Thinking Learning Tutor**를 사용하세요.
* 접근성 요구사항과 포용적 설계 고려 사항을 위해**Accessibility Planner**를 사용하세요.
* 접근성 준비 상태에 대한 검토를 위해 **Accessibility Reviewer**를 사용하세요.
* 책임 있는 AI 요구사항, 위험, 가드레일을 위해 **RAI Planner**를 사용하세요.
* 책임 있는 AI 검토를 위해 **RAI Reviewer**를 사용하세요.
* 간단한 솔루션 접근 방식, 트레이드오프, 아키텍처 노트를 구성하기 위해 **System Architecture Reviewer**를 사용하세요.
* 백로그 검토 후 GitHub Issues를 생성하거나 업데이트하기 위해 **GitHub Backlog Executor**를 사용하세요.
* 추가 검토, 위험 점검, 준비 상태 고려를 위해 **Security Planner**를 사용하세요.

### 시작하기 가이드

> [!TIP]
> 모든 역할에 걸쳐 솔루션을 Microsoft Marketplace와 Microsoft 365
> Copilot Agent Store에 게시할 수 있도록 설계하세요. Microsoft
> Marketplace에 솔루션을 게시하는 것은 도달 범위를 확장하고, 고객
> 조달을 단순화하며, 리워드와 인센티브, GTM(시장 진출) 혜택을 얻고,
> 반복적인 수익 기회를 만드는 가장 빠른 방법 중 하나입니다.
>
> 두 목적지 모두에서 패키징, 발견, 검토를 지원할 만큼 결과물을 명확하게
> 유지하세요.

## 주제 전문가(SME) 트랙

### 목표

누군가 무엇을 설계하거나 구축하기 전에 비즈니스 진실을 포착하세요.

### 컨텍스트 만들기
1. 선택한 사용 사례에 대해 정책 문서, SOP, 프로세스 다이어그램, 메모, 문서 참조, PDF, 스크린샷, 이미지와 같은 사용 가능한 증거를 수집하세요.
2. 워크샵 사례의 경우, 합성 데이터 또는 공개 소스 파일을 `policies/`, `sops/`, `process-diagrams/`와 같이 유형별로 정리하여 수동으로 관리하는 `./copilot-tracking/research/workshop-input/` 폴더에 보관하세요. 원본 다이어그램 파일은 렌더링된 이미지 옆에 보관하세요.
3. 실제 프로덕션 사례의 경우, 고객, 규제 대상, 기밀, 프로덕션 증거를 저장소에 복사하지 마세요. 통제된 SharePoint 또는 OneDrive 라이브러리, 접근 제어가 적용된 Azure Blob Storage 또는 ADLS, 승인된문서 관리 시스템, 또는 보안 데이터 룸과 같은 승인된 시스템에 보관하세요. 분류, 보존, 접근 권한을 확인한 후 신뢰할 수 있는 읽기 가능 경로 또는 통제된 링크를 `/rpi-research`에 제공하세요.

### 워크샵 입력으로서의 Marketplace Lean Canvas

PM, 디자인, 기술 트랙이 시작되기 전에 SME의 빠른 워크샵 입력으로 이 린 캔버스를 사용하세요. 목적은 비즈니스 현실을 나머지 팀이 검토하고 다듬을 수 있는 간결하고 공유된 형식으로 포착하는 것입니다.

각 항목을 증거 기반으로 유지하세요. 데이터를 알 수 없는 경우 `Unknown`을 기록하고 출처나 필요한 결정을 메모하세요. 고객 세그먼트, 가격, 지표를 지어내지 마세요.

| 비즈니스 문제 또는 어려움 | 목표 고객 또는 사용자 | 고유 가치 제안 |
|---|---|---|
| 오늘날 비용이 많이 들고, 위험하고, 느리고, 좌절스러운 문제는 무엇인가? 아무것도 하지 않을 때의 비용은 무엇인가? | 누가 영향을 받는가? 누가 비용을 지불하는가? 주요 의사 결정자는 누구인가? | 이 제안이 의미 있게 더 낫고, 더 빠르고, 더 안전하거나, 더 저렴한 이유는 무엇인가? |

| 솔루션 또는 핵심 오퍼 | 유통 또는 채널 | 수익 모델 또는 가치 획득 |
|---|---|---|
| 문제를 해결하는 오퍼, 워크플로우, 서비스는 무엇인가? 최소 실행 가능 버전은 무엇인가? | 고객은 어떻게 오퍼를 발견하고, 구매하고, 받는가? 어떤 채널과 파트너가 중요한가? | 수익 흐름, 가격 모델, 상업적 가정은 무엇인가? |

| 비용 구조 | 핵심 지표 및 성공 척도 | 경쟁 우위 또는 차별화 요소 |
|---|---|---|
| 주요 비용 동인, 종속성, 운영 제약은 무엇인가? | 가치를 증명할 지표는 무엇인가: 채택, 속도, 품질, 비용 절감, 위험 감소, 처리량, 유지율? | 이 이니셔티브에 지속적인 우위를 주는 것은 무엇인가: 정책 적합성, 워크플로우 깊이, 데이터 접근, 신뢰, 낮은 마찰, 도메인 전문성? |

#### 캔버스 작성을 위한 SME 및 제품 매니저 프롬프트

```text
/rpi-research
session-context=.copilot-tracking/research/[date]/[session-name]-session-context.md.
Read the topic and evidence root from the session context. Use the business
evidence, policies, process notes, and user-impact notes in the research
artifact.
Draft a concise lean canvas for an [FSI relationship manager assistant]. Capture
the problem, target customer segments, value proposition, core offering,
channels,
revenue model, costs, success metrics, and unique advantage. Separate facts from
assumptions and flag each unknown item for follow-up. Keep the wording grounded
in evidence, not marketing language. Save the output under
./copilot-tracking/research/workshop-input/leancanvas.md
```
#### 결과 체크리스트

1. 영향을 받는 사용자와 영향을 포함한 문제 정의.
2. 목표 고객 또는 사용자 세그먼트와 의사 결정자.
3. 비즈니스 증거에 근거한 가치 제안.
4. 최소 실행 가능 오퍼 또는 워크플로우.
5. 알려진 수익, 비용, 운영 가정.
6. 성공 지표와 이를 검증하는 데 필요한 비즈니스 증거.
7. 다음 역할이 해결해야 할 위험, 종속성, 미지수.

### 리서치 시작
1. 시나리오와 사용 가능한 증거에 대해 `/rpi-research`를 실행하세요:

   ```text
   /rpi-research
   session-context=.copilot-tracking/research/[date]/[session-name]-session-context.md.
   Read the topic and evidence root from the session context and theworkshop-input.
   Research the supplied scenario, policies, process notes, and supporting materials. Identify evidence-backed business facts, affected users, business rules, constraints, known failure cases, AI guardrails, open questions, and credible alternatives or counter-evidence.
   Save the dated primary research artifact under `.copilot-tracking/research/`. Keep the scope to context discovery.
   ```

   로컬로 동기화되고 접근이 통제된 OneDrive 폴더를 사용하는 프로덕션 사례의 경우, 신뢰할 수 있는 증거 루트를 명시적으로 제공하세요:

   ```text
   /rpi-research
   session-context=.copilot-tracking/research/[date]/[session-name]-session-context.md.
   Read the topic and OneDrive evidence root from the session context. Research
   the policies, SOPs, process diagrams, notes, PDFs, and screenshots in that
   folder. Identify evidence-backed business facts, affected users, business
   rules, constraints, known failure cases, AI guardrails, open questions, and
   credible alternatives or counter-evidence. Save the dated primary research
   artifact under `.copilot-tracking/research/`. Do not copy source files into
   the
   repository; cite the source filename and controlled location in the research
   artifact.
   ```

   조직의 권한, 보존, 분류 정책이 적용되는 OneDrive 폴더를 사용하세요.
   프로덕션 증거에는 공개 공유 링크나 개인 OneDrive 폴더를 사용하지
   마세요.

1. `.copilot-tracking/research/`에 생성된 리서치 아티팩트를 검토하세요.이것이 귀하의 영구적인 증거 추적입니다.
2. 문제 정의, 영향을 받는 사용자, 비즈니스 영향, 비즈니스 규칙, 알려진 실패 사례, AI 가드레일과 같은 주요 발견 사항을 컨텍스트 문서에 추출하여 기록하세요. 추적성을 위해 리서치 아티팩트를 참조하세요.
3. 사실을 가정, 결정, 미해결 질문과 분리하세요. 가능한 경우 지원 자료를 링크하거나 참조하세요.
4. 구조가 필요하다면 **BRD Builder** 또는 **PRD Builder**에게 비즈니스 또는 제품 요구사항 개요 초안을 요청하세요. 메모를 공유하는 것으로 시작하여 문제 정의, 비즈니스 목표, 범위, 가정, 수락 기준을 만들도록 요청하세요.

   팀이 비즈니스 사례, 이해관계자, 결과, 제약, 결정 컨텍스트를 수립해야 할 때 **BRD Builder**를 사용하세요:

   ```text
   Select the /BRD Builder agent. Session context:
   .copilot-tracking/research/[date]/[session-name]-session-context.md.
   Read the topic from the session context, then use its evidence references and
   research artifact. Draft a concise business requirements outline covering the
   business problem, affected stakeholders, measurable business outcomes, scope,
   non-goals, business rules, constraints, risks, assumptions, dependencies, and
   unresolved questions. Save the BRD draft and its session state under
   `.copilot-tracking/brd-sessions/`. Separate evidence-backed facts from
   assumptions and proposed decisions. Do not invent customer facts, policy
   requirements, metrics, or implementation commitments. Mark the document as a
   draft for human review and include testable acceptance criteria where they
   clarify the business outcome.
   ```

   팀이 제품 동작, 사용자 요구, 기능 요구사항, 비기능 요구사항, 수락 기준이 필요할 때 **PRD Builder**를 사용하세요:

   ```text
   Select the /PRD Builder agent. Session context:
   .copilot-tracking/research/[date]/[session-name]-session-context.md.
   Read the topic from the session context, then use its research artifact and
   business requirements references. Draft a concise product requirements
   outline
   covering target users, jobs to be done, user journeys, in-scope and
   out-of-scope
   behavior, functional requirements, non-functional requirements, data and AI
   guardrails, known failure cases, accessibility needs, success metrics,
   dependencies, and testable acceptance criteria. Save the PRD draft and its
   session state under `.copilot-tracking/prd-sessions/`. Preserve citations or
   references to the supporting evidence. Separate facts from assumptions,
   decisions, and open questions. Do not invent customer data, policy
   requirements, or unsupported technical details. Mark the document as a draft
   for human review.
   ```

   프로덕션 증거의 경우, 승인된 소스 경로나 통제된 링크를 컨텍스트로 제공하세요. 승인된 환경이 허용하지 않는 한 민감한 소스 콘텐츠를 저장소에 붙여넣거나 복사하지 마세요.

### 결과물

1. **리서치 아티팩트**(`.copilot-tracking/research/`): 사실, 가정,
   제약, 미해결 질문을 담은 증거 기반 리서치 결과.
2. **BRD 초안**(`.copilot-tracking/brd-sessions/`): 비즈니스 요구사항,
   이해관계자, 결과, 제약, 수락 의도.
3. **요구사항 초안**(`.copilot-tracking/prd-sessions/`): 테스트 가능한
   수락 기준을 갖춘 제품 요구사항.

## 디자인 트랙

### 목표

비즈니스 컨텍스트를 명확한 사용자 경험과 문제에 대한 공유된 이해로
변환하세요.

### 단계

1. `.copilot-tracking/research/` 아래 SME가 만든 컨텍스트 패키지를
   읽으세요.
2. 최종 경험 초안을 작성하기 전에 공유 컨텍스트에 디자인 증거를
   추가하세요. 관련 사용자 리서치, 화면 스케치, 와이어프레임을 동일한
   프로젝트 폴더에 담아 다음 역할이 증거 추적의 일부로 검토할 수 있도록
   하세요. 실무적인 패턴은 다음과 같습니다:

   * 시나리오를 위해 `.copilot-tracking/dt/<project-name>/` 아래에
     디자인 작업 폴더를 만드세요.
   * 연구 목표, 참가자, 관찰, 핵심 테마, 미해결 질문을 담은 간단한
     `user-research.md`를 추가하세요.
   * 로파이 화면 스케치, 주석이 달린 목업, 또는 Figma 파일 링크를 위한
     `screens/` 또는 `wireframes/` 폴더를 추가하세요.
   * 사용자 흐름, 주요 어려움, 결정 사항을 요약하는
     `journey-notes.md` 또는 `experience-draft.md`를 추가하세요.
   * 각 아티팩트에 증거 유형, 날짜, 출처, 관찰됨/보고됨/가정됨/미해결
     질문 여부를 라벨링하세요.
   * 고객 데이터 또는 규제 대상 데이터는 저장소 밖에 두세요. 디자인
     아티팩트가 보호되는 데이터에 기반한다면 민감한 콘텐츠를 복사하는
     대신 승인된 소스 위치를 참조하세요.

   예시 패턴:

```text
.copilot-tracking/dt/<project-name>/
  user-research.md
  journey-notes.md
  experience-draft.md
  screens/
    home-screen-sketch.png
    account-summary-wireframe.png
  wireframes/
    customer-conversation-prep.fig
```

3. 리서치와 디자인 아티팩트를 사용하여 가정이 아닌 관찰된 사용자
   요구에 디자인 결정을 근거하세요. 팀이 나중에 검토할 수 있도록
   미해결 질문과 가정의 목록을 유지하세요.
4. 최종 사용자 및 이해관계자와 함께 에이전틱 AI 기능을 브레인스토밍하기
   위한 design thinking
   [**Microsoft AI Discovery Cards 워크샵**](https://aka.ms/AIDiscoveryCards)을
   계획하세요.
5. 하나의 주요 사용자와 하나의 핵심 과업(job to be done)을
   선택하세요.
6. 현재 여정을 매핑하고 어려움을 식별하세요.
7. 의도한 솔루션으로 미래 여정을 설명하세요.
8. 접근성과 책임 있는 AI 요구사항을 추가하세요.
9. 첫 초안이 필요하다면 **UX UI Designer**에게 문제를 간단한 사용자
   여정과 경험 개요로 전환하도록 요청하세요.
   `.copilot-tracking/research/` 아래의 컨텍스트 패키지를 선택하고
   GitHub Copilot Chat에서 다음 프롬프트를 사용하세요:

```text
"Turn these notes into a simple user journey, experience outline, and key pain
points for this scenario. Save the reviewed experience draft under
`.copilot-tracking/dt/`."
```

10. 팀에 안내된 대화가 필요하다면 **Design Thinking Coach**에게 기회를
    구성하고 가정에 도전하도록 요청하세요.

```text
"Coach me through a short design thinking session for this scenario. Help me
frame the problem, identify user needs, and define a focused opportunity area
for the solution."
```

11. 팀에 학습 지원이나 더 명확한 다음 단계가 필요하다면
    **Design Thinking Learning Tutor**에게 방법을 설명하고 메모를 간단한
    디자인 아티팩트로 전환하도록 도움을 요청하세요.

```text
"Act as a Design Thinking Learning Tutor. Explain the next design thinking step
for this scenario and help me turn my notes into an insight, opportunity
statement, or user journey outline."
```

12. **Accessibility Planner**와 **Accessibility Reviewer**를 사용하여
    접근성 요구사항을 드러내고 초안의 공백을 검토하세요.
   `.copilot-tracking/dt/` 아래의 경험 초안을 선택하고 Accessibility
   Planner에게 다음과 같이 프롬프트하세요:

```text
"Review the experience draft under `.copilot-tracking/dt/` and identify
accessibility requirements, user needs, follow-up questions for implementation,
and updates to the draft."
```

13. **RAI Planner**와 **RAI Reviewer**를 사용하여 책임 있는 AI
    요구사항, 가드레일, 검토 결과를 포착하세요.
   `.copilot-tracking/dt/` 아래의 경험 초안을 선택하고 **RAI Planner**
   프롬프트를 사용하세요:

```text
"Review the experience draft under `.copilot-tracking/dt/` and identify
responsible AI requirements, potential harms, mitigation ideas, and updates to
the draft."
```

14. 팀이 Figma를 사용한다면, 경험 초안에 Figma 파일, 와이어프레임,
    디자인 아티팩트에 대한 링크나 참조를 포함하세요. Figma 결과물을
    사용자 흐름, 화면, 디자인 결정의 증거로 사용하고, 해당 아티팩트가
    워크샵 핸드오프를 어떻게 뒷받침하는지 메모하세요.

#### Figma MCP와 FigJam 연결하기

Figma MCP는 선택 사항입니다. 디자인 증거, 사용자 흐름, 와이어프레임,
워크샵 핸드오프를 위해 GitHub Copilot을 Figma 파일과 FigJam 보드에
연결합니다.

15. 작업 공간 루트에서 `.vscode/mcp.json`을 만들거나 여세요.
16. Figma MCP 서버를 추가하세요:

    ```json
    {
       "servers": {
          "figma": {
             "type": "http",
             "url": "https://mcp.figma.com/mcp"
          }
       }
    }
    ```

17. 파일을 저장하고, Copilot Chat에 MCP 서버가 나타나지 않으면 VS
    Code를 다시 로드하세요.
18. 관련 디자인 프롬프트(예: `dt-figma-export`)에서 Figma 또는 FigJam
    작업을 시작하세요.
19. 첫 호출에서 브라우저 기반 Figma OAuth 로그인을 완료하고 워크샵에
    사용되는 파일이나 보드에 대한 접근 권한을 부여하세요.
20. 결과로 생성된 Figma 또는 FigJam URL을 경험 초안에서 아티팩트
    유형, 날짜, 증거 상태, 그것이 뒷받침하는 사용자 흐름이나 디자인
    결정과 함께 참조하세요.

Figma MCP 서버는 로컬 설치가 필요하지 않습니다. 지속적인 사용을 위해서는
Professional, Organization, Enterprise 플랜의 Dev 또는 Full 시트가 있는
Figma 계정이 필요합니다. 전체 작업 공간 구성 및 문제 해결 가이드는
[MCP 서버 구성](mcp-configuration)을 참고하세요.

21. Microsoft 365 Copilot Agent Store에 게시하기 위한 사용 사례를
    식별하고 검증하세요.
   `.copilot-tracking/dt/` 아래의 경험 초안을 선택하고 UX UI
   Designer에게 다음과 같이 프롬프트하세요:

```text
"How would end users benefit from Microsoft 365 Copilot integrated to this
scenario? What research would I need to run to validate it? Update the
experience
draft under `.copilot-tracking/dt/`."
```

22. 경험을 Microsoft Marketplace와 Microsoft 365 Copilot Agent
    Store를 위해 어떻게 패키징하고, 발견 가능하게 하고, 검토 가능하게
    할지 메모하세요.
23. 성공 기준과 미해결 질문을 정의하세요.
4. 검토된 결과를 경험 초안으로 `.copilot-tracking/dt/` 아래에
   저장하세요.

### 결과물

`.copilot-tracking/dt/`: 사용자 경로, 어려움, 디자인 제약을 포착한 사용자 경험 초안.

다음 단계: [**역할별 트랙 Part2: 아키텍처 설계, 백로그**](partner-workshop-role-tracks-2.md)를 진행하세요.
