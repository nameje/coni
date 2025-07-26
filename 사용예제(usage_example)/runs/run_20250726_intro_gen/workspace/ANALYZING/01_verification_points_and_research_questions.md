# 검증 및 리서치 필요 항목 분석

## 1. '과정' 섹션
- **사용자 아이디어 1:** LLM 작업을 세분화(Task)하고, 이를 단계(Stage, Phase)별로 묶어 순차적으로 실행하면 결과물의 만족도가 높아지고 일관성을 유지할 수 있다.
  - **검증 포인트:** 이 가설은 실제 AI 에이전트 연구에서 통용되는 개념인가?
  - **리서치 질문:**
    - "LLM-based agent workflow" 또는 "agentic workflow"에서 'Task decomposition'의 중요성에 대한 연구가 있는가?
    - "Chain-of-Thought (CoT)", "Tree-of-Thought (ToT)", "Graph-of-Thought (GoT)" 등과 같은 프롬프팅/에이전트 기법이 이러한 세분화 및 구조화와 어떤 관련이 있는가?
    - LLM 에이전트의 'Hierarchical Planning(계층적 계획)'은 성능에 어떤 영향을 미치는가? 관련 논문이나 프로젝트가 있는가?

- **사용자 아이디어 2:** 플래너, 익스큐터 등 역할을 분리하고, 파일 시스템(workspace)을 공유 메모리로 사용하는 방식이 인공신경망 구조와 유사하다.
  - **검증 포인트:** 이 아키텍처 비유는 타당한가? 실제 멀티 에이전트 시스템은 어떻게 통신하고 협력하는가?
  - **리서치 질문:**
    - "Multi-Agent LLM systems architecture"의 최신 동향은 무엇인가?
    - 에이전트 간 통신 방법(Inter-agent communication)에는 어떤 것들이 있는가? (e.g., message passing, shared memory, blackboard systems)
    - MetaGPT, AutoGen, ChatDev와 같은 실제 멀티 에이전트 프레임워크는 어떤 구조와 통신 방식을 사용하는가? 사용자의 제안과 어떤 점이 유사하고 다른가?

## 2. '문제점' 섹션
- **사용자 아이디어 3:** 최신 LLM들이 '사고'보다 '행동'을 우선으로 답하는 경향이 있어, 강제로 사고 과정(철학, 방법 등)을 주입해야 한다.
  - **검증 포인트:** 이것이 실제 관찰되는 LLM의 행동 변화인가? 'Alignment'나 'Instruction Tuning'의 영향일 수 있는가?
  - **리서치 질문:**
    - "LLM alignment tax" 또는 "instruction tuning side effects"와 관련된 연구가 있는가?
    - 최신 모델들이 더 "helpful and harmless"하게 조정되면서, 복잡하고 다단계적인 추론 능력이 저하되었다는 주장이 있는가?
    - "Constitutional AI"와 같은 접근법이 모델의 행동 경향에 어떤 영향을 미치는가?

## 3. '확장 가능성' 및 '생각' 섹션
- **사용자 아이디어 4:** 이 행동규범 구조를 재귀적으로 적용하여, Task 단위의 익스큐터를 하위 에이전트로 대체하면 인간 조직과 유사한 계층적 에이전트 시스템을 만들 수 있다.
  - **검증 포인트:** 이러한 '재귀적 에이전트' 또는 '에이전트 조직' 개념이 실제로 연구되고 있는가?
  - **리서치 질문:**
    - "Recursive LLM agents" 또는 "Hierarchical agent teams"에 대한 연구 프로젝트나 논문이 있는가?
    - AI 에이전트를 사용하여 가상 소프트웨어 회사를 시뮬레이션하는 'ChatDev'와 같은 프로젝트는 어떤 구조적 특징을 가지는가?
    - 이러한 계층적 구조가 가질 수 있는 장점(e.g., 복잡성 관리, 전문화)과 단점(e.g., 통신 오버헤드, 오류 전파)은 무엇으로 논의되는가?

- **사용자 아이디어 5:** 이 행동규범의 구조를 실제 인공신경망 아키텍처에 적용하여 계층적/연속적 신경망을 만들 수 있다.
  - **검증 포인트:** 추상적인 에이전트 아키텍처와 실제 뉴럴 네트워크 아키텍처는 개념적으로 연결될 수 있는가?
  - **리서치 질문:**
    - "Modular neural networks" 또는 "Hierarchical reinforcement learning"과 같은 분야에서, 네트워크의 모듈이나 계층이 에이전트의 역할/기능과 유사하게 분리되는 사례가 있는가?
    - 에이전트의 '실행의 사슬(Chain of Execution)'을 신경망의 '가중치'로 비유했는데, 이를 더 구체적으로 뒷받침하거나 반박할 수 있는 신경망 이론이 있는가? (e.g., "dynamic routing in capsule networks", "attention mechanisms as a form of information routing")
