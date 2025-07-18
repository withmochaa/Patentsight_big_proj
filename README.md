<div align="center">

# 특허톡 (Pat-talk): AI 기반 출원 서류 자동 점검 및 우선심사 분류 시스템
**AIVLE 5기 AI Track 7조 빅프로젝트**

<p>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
    <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
</p>
</div>

---

## 📖 프로젝트 개요 (Project Overview)
특허톡 (Pat-talk)은 특허 출원 프로세스의 복잡성과 비효율성을 해결하기 위해 개발된 **AI 어시스턴트 서비스**입니다. 본 프로젝트는 특허 출원인과 심사관 모두를 지원하여, 서류 준비 과정의 오류를 90%까지 줄이고 심사 업무의 효율을 높여 궁극적으로 특허 등록 성공률을 향상시키는 것을 목표로 합니다. AI 모델을 통해 서류를 자동 점검하고, 조건 충족도에 따라 우선심사 대상을 분류하여 특허 행정의 혁신을 도모합니다.

---

## ✨ 주요 기능 (Key Features)
### 기능적 요구사항 (Functional Requirements)
| 대상 고객 | 기능 항목 | 상세 요구 사항 |
| :--- | :--- | :--- |
| **출원인** | AI 기반 서류 점검 | 명세서, 청구항, 도면 등 서류 전반의 형식/내용상 오류를 자동으로 탐지하고, 필수 기재 항목 누락 여부를 체크합니다. |
| | 초안 생성 및 보완 | AI 어시스턴트가 청구항 및 명세서의 초안 생성을 돕고, 발견된 오류에 대한 보완 가이드를 제공합니다. |
| | 거절 위험도 예측 | 작성된 서류를 기반으로 심사 거절 위험도를 예측하고 사전에 안내하여 보완할 수 있도록 지원합니다. |
| **심사관** | 우선심사 자동 분류 | AI가 서류의 조건 충족도를 점수화(Scoring)하여 우선순위를 자동으로 매기고, 우선순위가 높은 순서대로 담당자에게 배분합니다. |
| | 자연어 기반 특허 검색 | 대화형 챗봇을 통해 자연어로 질문하듯 유사 특허를 검색하고, 기술 구조와 문맥적 의도를 함께 반영하여 정확도를 높입니다. |
| | 의견서 초안 자동 생성 | AI가 분석 결과에 기반하여 거절 이유 통지서 등 심사 의견서의 초안을 자동으로 생성하여 심사관의 반복 업무를 줄여줍니다. |

### 기대 효과 (Expected Outcomes)
- **시간 및 비용 절감**: 출원 서류의 초안 생성 및 오류 탐지 자동화로 출원 준비 시간을 1건당 평균 3~5시간 단축할 수 있습니다.
- **등록 성공률 향상**: 형식적/논리적 오류를 사전에 방지하여 특허 등록 성공률을 약 10~20%p 향상시키는 것을 목표로 합니다.
- **업무 효율성 증대**: 심사관의 반복적인 서류 검토 및 통지서 작성 업무를 자동화하여 실질 심사에 더욱 집중할 수 있는 환경을 제공합니다.
- **심사의 객관성 확보**: 기존 평가의 주관적 판단 요소 비중(30%)을 AI 지원을 통해 약 10~15% 수준까지 축소하여 공정성을 높입니다.

---

## 🏛️ 시스템 설계 및 구조 (System Design & Architecture)
프로젝트의 전체적인 흐름과 구조는 다음과 같습니다.

### 1. 전체 서비스 흐름도 (Overall Service Flow)
*출원인과 심사관의 상호작용을 중심으로 한 AI 기반 특허 심사 프로세스입니다.*
<div align="center">
  <img src="https://raw.githubusercontent.com/withmochaa/Patentsight_big_proj/main/images/1.png" alt="전체 서비스 흐름도" width="80%">
</div>

### 2. 사용자 인터페이스 및 상호작용 흐름 (UI & Interaction Flow)
*사용자가 시스템에 접속하여 AI 챗봇과 상호작용하며 서비스를 이용하는 상세 흐름입니다.*
<div align="center">
  <img src="https://raw.githubusercontent.com/withmochaa/Patentsight_big_proj/main/images/2.png" alt="사용자 인터페이스 및 상호작용 흐름" width="80%">
</div>

### 3. 상세 UI 설계 (Wireframe)
*주요 기능에 대한 와이어프레임 및 상세 화면 설계입니다.*
<div align="center">
  <img src="https://raw.githubusercontent.com/withmochaa/Patentsight_big_proj/main/images/4.png" alt="상세 UI 설계" width="80%">
</div>

### 4. 데이터베이스 설계 (ERD)
*서비스 운영에 필요한 데이터베이스의 테이블 구조 및 관계(ERD)입니다.*
<div align="center">
  <img src="https://raw.githubusercontent.com/withmochaa/Patentsight_big_proj/main/images/3.png" alt="데이터베이스 ERD" width="80%">
</div>

---

## 👥 팀원 및 역할 (Team & Roles)
| 역할 (Role) | 담당자 (Member) | 주요 업무 (Responsibilities) |
| :--- | :--- | :--- |
| 👨‍💻 **총괄 및 모델링** | `남경탁(조장)` | 프로젝트 총괄, 백엔드 및 AI 모델링, 영상 제작 |
| ⚙️ **백엔드 및 데이터** | `김강민` | 백엔드, 데이터베이스, AI 모델링 |
| 🎨 **프론트엔드 및 모델링** | `나성원` | 프론트엔드(FE), 백엔드(BE), 데이터, AI 모델링, PPT |
| 🚀 **프론트엔드 및 데이터** | `박채은` | 프론트엔드, 백엔드, 데이터, AI 모델링 |
| 📝 **프론트엔드 및 기획** | `정지원` | 프론트엔드, 백엔드, 데이터, PPT |
| 📊 **모델링 및 문서화** | `채윤승` | 백엔드, 데이터, AI 모델링, 영상 제작, PPT |

---

## 🛠️ 기술 스택 및 데이터 (Tech Stack & Data)
| 구분 | 기술 및 데이터 |
| :--- | :--- |
| **AI & Modeling** | `Multimodal Models` `Bidirectional Transformer` `Local LLM (탐색)` |
| **Backend** | `Python` `FastAPI` (예상) |
| **Frontend** | `React` `JavaScript` (예상) |
| **Data Source** | `KIPRIS API` (특허 공보, 행정 문서, 가이드라인) <br> `자체 수집 데이터` (사용자 피드백 로그) |
| **Planning & Docs**| `Notion` `Canva` |

---

## 🗓️ 프로젝트 일정 (Project Schedule)
본 프로젝트는 2주간 진행되며, 기획/설계 단계와 구현 단계로 나뉩니다.
| 주차 | 주요 수행 과업 | 기한 | 주요 활동 |
| :--- | :--- | :--- | :--- |
| **1주차** | 과제 발굴 및 서비스 기본 기획 | ~ 07/09 | - 팀별 아이디어 도출 및 프로젝트 주제 선정<br>- 과제 정의서 및 요구사항 정의서 작성<br>- 코칭을 통한 아이디어 및 기획 검토 |
| **2주차** | 서비스 기획 구체화 및 시스템 상세 설계 | ~ 07/18 | - 1주차 피드백 반영 및 2주차 상세 계획 수립<br>- 아키텍처, 서비스 플로우, ERD, UI/UX 설계<br>- 전체 산출물 최종 검토 및 제출 |

---

<div align="center">
    <img src="https://raw.githubusercontent.com/withmochaa/Patentsight_big_proj/main/images/aivle_logo.png" alt="AIVLE Logo" width="400">
</div>
