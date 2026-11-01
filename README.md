<div align="center">

  <!-- Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,11,21,31&height=200&section=header&text=eethsc+👋&fontSize=42&fontAlignY=38&desc=Harness+%26+Search+Engine+Engineer+%7C+Agentic+AI+Architect&descAlignY=62&descSize=16" width="100%" alt="Header Banner" />

  <!-- Dynamic Typing Subtitle -->
  <a href="https://github.com/eethsc">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&duration=2500&pause=1000&color=38BDF8&center=true&vCenter=true&width=680&height=40&lines=Agent+Harness+Engineering+%26+Autonomous+Causal+Verification;Advanced+Hybrid+RAG+(Kiwi+BM25+%2B+Voyage+Dense+%2B+Cross-Reranker);Multi-Domain+Search+Engines+(Tavily+%C2%B7+Exa+%C2%B7+Firecrawl+%C2%B7+Scrape.do);AI+Semiconductor+%26+EDA+Automation+via+Closed-Loop+Agents" alt="Typing SVG" />
  </a>

  <p align="center">
    <a href="https://github.com/eethsc?tab=repositories"><img src="https://img.shields.io/badge/Focus-Harness%20%26%20Search%20Engine-6366f1?style=flat-square&logo=target&logoColor=white" alt="Focus" /></a>
    <a href="https://github.com/eethsc?tab=repositories"><img src="https://img.shields.io/badge/Architecture-Agentic%20AI%20%26%20RAG-0ea5e9?style=flat-square&logo=diagram-next&logoColor=white" alt="Architecture" /></a>
    <img src="https://komarev.com/ghpvc/?username=eethsc&label=Profile%20Views&color=0284c7&style=flat-square" alt="Profile Views" />
  </p>

</div>

---

### 👨‍💻 About Me

> **"신뢰할 수 있는 에이전트 하네스(Harness)와 노이즈 없는 고정밀 검색 엔진을 구축합니다."**

LLM이 실전 프로덕션에서 동작하기 위해 반드시 해결해야 할 **2가지 핵심 축(검색 정확도와 검증 거버넌스)**을 깊이 있게 파고드는 소프트웨어 엔지니어입니다.

- 🔎 **Search & Retrieval Engineering:** Sparse(BM25)와 Dense Vector의 단순 결합을 넘어, 형태소 단위 사전 인덱싱, Cross-Encoder 리랭킹, 그리고 4대 웹 검색 엔진을 아우르는 **도메인 특화 고성능 검색 파이프라인**을 설계합니다.
- 🛡️ **Harness & Verification Engineering:** 에이전트의 환각(Hallucination)과 수렴 실패를 원천 차단하기 위해, 인과 의존성 그래프 기반의 게이트키퍼와 **평가·검증 전용 하네스(Dual-Harness²)** 구조를 엔지니어링합니다.
- ⚡ **AI Semiconductor & EDA Automation:** 극도로 엄격한 도메인 지식이 요구되는 반도체/회로 물리 영역을 **순수 SW/Agentic AI 관점에서 데이터시트 파싱 ➔ 지식 그래프 추출 ➔ 코드 자율 합성 ➔ 폐루프 물리 시뮬레이션 검증**으로 자동화한 AI 반도체 프로젝트를 성공적으로 완수한 경험이 있습니다.

---

### 🛠️ Core Technology Stack

<div align="center">

#### AI Search & Retrieval (RAG & Web Scraping)
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=python,fastapi,postgres" alt="Search Stack" />
</a>
<br/>
<p align="center">
  <img src="https://img.shields.io/badge/Kiwi_BM25-한국어_형태소_사전_인덱싱-4B5563?style=flat-square&logo=python&logoColor=white" alt="Kiwi" />
  <img src="https://img.shields.io/badge/Voyage_AI-Dense_Embedding_%26_Rerank--2-7C3AED?style=flat-square" alt="Voyage" />
  <img src="https://img.shields.io/badge/ChromaDB-Vector_Store-E11D48?style=flat-square" alt="ChromaDB" />
  <img src="https://img.shields.io/badge/Multi--Web_Search-Tavily_%C2%B7_Exa_%C2%B7_Firecrawl_%C2%B7_Scrape.do-0EA5E9?style=flat-square" alt="Web Search" />
</p>

#### Backend, Cloud & Production
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=ts,js,nodejs,react,vite,docker,supabase,githubactions,git,linux" alt="Full Stack & Cloud" />
</a>

</div>

---

### 🏛️ Engineering Pillars & Key Systems

| 핵심 영역 | 설계 아키텍처 및 구현 성과 | 기술 스택 |
| :--- | :--- | :--- |
| **🔎 Hybrid RAG Engine** | **KlaWde: 고성능 학사 인텔리전스 챗봇 시스템**<br>• **Pre-indexing Baking:** 런타임 CPU 병목을 없애기 위해 오프라인 빌드 타임에 Kiwi 형태소 기반 BM25 피클 객체 사전 캐싱 (로드 시간 0.1s)<br>• **Cross-Attention Reranking:** 1차 추출 40개 후보군(Sparse 20 + Dense 20)을 Voyage `rerank-2`로 재정렬하여 `top_n=4` 정밀 압축<br>• **Context Reconstruction:** 정밀 Child 청크에서 1,500자 Parent 윈도우 문맥 복원 및 멀티턴 Query Rewriting<br>• **GIL 격리 비동기 아키텍처:** 프론트엔드와 무거운 RAG 연산 간 교착 상태를 방지하는 비동기 데몬 스레드 & 디스크 세션 폴링 | `Python` `Streamlit` `Kiwi` `VoyageAI` `ChromaDB` `Gemini` `SQLite` |
| **🌐 Multi-Domain Search Engine** | **Event Hub: 4대 골든 스택 에이전틱 웹 전수조사 파이프라인**<br>• **다중 도메인 탐색:** 심층 RAG(Tavily), 시맨틱 뉴럴 탐색(Exa), 마크다운 정찰(Firecrawl), WAF/보안 우회(Scrape.do)를 통합 오케스트레이션<br>• **무중단 운영:** GitHub Actions 클라우드 스케줄러(매일 06:00 KST)로 7,000+건 데이터 자동 수집 및 정제<br>• **보안 클라우드 DB 연동:** Supabase PostgreSQL RLS(Row Level Security) 접근 제어 및 실시간 대량 Upsert 파이프라인 | `Node.js (Native)` `Supabase` `PostgreSQL (RLS)` `GitHub Actions` `PWA` |
| **🛡️ Agent Harness & AI 반도체** | **Dual-Harness²: 폐루프 자율 합성 및 4단계 인과 검증 시스템**<br>• **에이전트 거버넌스 하네스($C_1\sim C_8$):** NousResearch Hermes Agent 코어 위에 서브서킷 스킬 및 수렴 함정 장기 메모리(`MEMORY.md`) 자율 관리<br>• **PDG 4단계 인과 검증 하네스($V_1\sim V_3$):** Stage 0(토폴로지) $\to$ Stage 1(전원/바이어스) $\to$ Stage 2(신호 전달) $\to$ Stage 3(스펙) 순차 강제 게이트로 환각 0% 달성<br>• **AI 반도체 자동화:** 비구조화 PDF 데이터시트에서 하드웨어 지식 그래프(HKG)를 추출하고 순수 물리 넷리스트를 자율 합성하는 E2E 파이프라인 | `Python` `Agent Harness` `Neuro-Symbolic` `SPICE/LTspice` `Playwright` |

---

### 📊 GitHub Activity & Language Analytics

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=eethsc&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eethsc&layout=compact&theme=tokyonight&hide_border=true" width="48%" alt="Top Languages" />
</div>

<div align="center" style="margin-top: 10px;">
  <img src="https://streak-stats.demolab.com/?user=eethsc&theme=tokyonight&hide_border=true" width="97%" alt="GitHub Streak" />
</div>

---

<div align="center">
  📫 <i>Open to discussions on Agent Harness Engineering, Advanced RAG, and Intelligent Search Architectures.</i>
</div>
