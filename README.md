<div align="center">

# Hyoju Kim · 김효주

**Statistics · AI Research · Applications**

데이터를 이해하고, 모델을 검증하며, 실제로 쓰이는 결과물을 만듭니다.

*Understanding data. Evaluating models. Building useful applications.*

[Projects](#-projects--프로젝트) · [Research](#-research--연구) · [Experience](#experience--경험) · [Tools](#tools--기술)

</div>

---

## About

인하대학교 대학원에서 데이터사이언스를 공부하고 있습니다. 통계적 모델링과 AI 연구를 바탕으로, 데이터 처리부터 모델 검증과 서비스 구현까지 경험을 넓혀왔습니다.

연구실에서는 국가연구개발과제의 제안서·계획서 작성, 진행 보고, 일정과 협업 조율을 함께 맡고 있습니다. 문제를 구체화하고 직접 구현해 확인한 결과를, 다른 사람이 활용할 수 있도록 정리하고 설명하는 일을 좋아합니다.

| Background | Focus |
|:---|:---|
| 경영학 → 통계학 → AI | 기술과 활용 목적을 함께 이해 |
| AI 연구 및 실험 | 성능과 적용 조건을 근거로 판단 |
| 서비스·파이프라인 개발 | 데이터와 모델을 실제 기능으로 연결 |
| 연구개발 과제 운영 | 계획·진행 상황·남은 과제를 명확히 공유 |

<details>
<summary>English introduction</summary>

<br>

I am a graduate student studying Data Science at Inha University. My work spans statistical modeling, AI research, data processing, model evaluation, and application development.

Alongside research, I support national R&D projects through proposal and project-plan preparation, progress reporting, scheduling, and coordination within the lab.

With an academic background in business administration, statistics, and AI, I enjoy defining problems, testing ideas through implementation, and communicating results so that others can use them.

</details>

---

## 🛠 Projects | 프로젝트

### • PetJJu
**반려동물 동반 제주여행 추천 챗봇**

`RAG` `Gemini API` `Pinecone` `Streamlit`

음식점·관광지·반려동물 편의시설 정보를 통합해 사용자 조건에 맞는 장소를 추천하는 팀 프로젝트입니다.

- **담당** — 데이터 전처리, 검색 필터링, 프롬프트 설계, 팀 일정 조율 및 최종 발표
- **구현** — 공통 데이터 구조, 조건 기반 검색·재검색, 검색 결과를 활용한 답변 생성
- **성과** — **2024 빅콘테스트 생성형 AI 분야 최우수상**
  · 한국지능정보사회진흥원장상

[View repository →](https://github.com/Hyoju-1/pet_jeju)

<details>
<summary>English overview</summary>

A team-built chatbot for pet-friendly travel in Jeju, combining restaurant, attraction, and pet-friendly facility data.

I worked on data preprocessing, search filters, prompt design, schedule coordination, and the final presentation. The project received the Excellence Award in the Generative AI category at BigContest 2024.

</details>

### • Marketing Decision Agent
**예측 결과를 마케팅 판단으로 연결하는 의사결정 지원 데모**

`Python` `pandas` `Upstage Solar` `Rule-based Decisions`

구매 가능성과 예상 행동 시점을 고객 분류·우선순위·추천 액션으로 변환하고, Solar를 활용해 판단 근거와 마케팅 문구를 생성합니다.

- **판단 구조** — 구매 의도와 시급성을 바탕으로 고객 분류 및 액션 추천
- **LLM 연계** — 선택적 LLM 판단 모드에서 정해진 후보 내 액션 선택
- **운영 고려** — 실패 시 규칙 기반 복귀, 우선순위와 최대 건수에 따른 호출 제한
- **결과물** — 고객 분류 CSV, 액션 계획 JSON, 요약 보고서 및 마케팅 문구

[View repository →](https://github.com/Hyoju-1/marketing_decision_agent)

<details>
<summary>English overview</summary>

A decision-support demo that translates purchase probabilities and estimated action timing into customer segments, priorities, and marketing recommendations.

It combines rule-based decisions with Solar-generated explanations and campaign copy. An optional LLM decision mode selects from predefined candidates, falls back to rules when needed, and limits calls by priority and record count.

The repository uses prediction outputs as inputs; model training and live campaign execution are outside its scope.

</details>

### • Voice Command Pipeline
**음성명령 해석 및 시스템 입력 패킷 생성**

`faster-whisper` `Local LLaMA 3 8B` `Parsing` `Validation`

음성을 텍스트로 변환하고 명령의 의미를 해석한 뒤, 후속 시뮬레이션이 요구하는 입력 패킷으로 연결합니다.

- **담당** — 처리 흐름 구성, 명령 해석 프롬프트, 정규화·검증 및 패킷 변환
- **처리 단계** — 음성 인식 → 항목 추출 → 정규화·검증 → 패킷 생성
- **검증 결과** — 준비된 MOVE·FIRES 명령 **9건 모두에서 패킷 생성 성공**
- **완료 결과** — 약 한 달 내 구현, 시연 및 결과물 제출

[View repository →](https://github.com/Hyoju-1/voice-command-pipeline)

<details>
<summary>English overview</summary>

A pipeline that converts spoken commands into structured simulation input packets.

I implemented command interpretation, normalization, validation, and packet conversion. Packet generation succeeded for all nine prepared MOVE/FIRES test cases. This result describes the prepared packet-generation tests, rather than unrestricted command understanding or full simulation operation.

</details>

### • RE:buy
**고객 행동 로그 기반 구매 가능성·시점 예측**

`Data Pipeline` `BERT4Rec` `Sequential Modeling` `BOAZ`

불필요한 광고 알림을 줄이기 위해 ‘누구에게 언제 안내할 것인가’를 구매 가능성과 구매 시점 예측 문제로 구체화한 BOAZ 팀 프로젝트입니다.

- **담당** — 문제 정의, 로그 표준화 파이프라인 및 예측 모델 설계, 최종 발표
- **데이터 처리** — 공통 입력 구조 정의, 컬럼 자동 매핑, 이벤트·시간 형식 정규화
- **모델링** — 이벤트·시간 정보 사전학습과 구매 가능성·시점 예측의 2단계 파인튜닝
- **평가 결과** — 마스킹 이벤트 복원 정확도 **79.85%**, 구매 시점 예측의 **24시간 이내 적중률 91.53%**

구매 여부 예측의 정밀도는 별도 개선 과제로 구분했으며, 알림 피로 감소와 매출 개선은 실제 서비스 환경에서 추가로 검증할 효과로 정리했습니다.

*Repository coming soon*

<!-- 저장소 생성 후 위 문구를 실제 Repository 링크로 교체하세요. -->

<details>
<summary>English overview</summary>

A BOAZ team project that translates the question “whom to notify, and when” into purchase-likelihood and purchase-timing prediction tasks.

I worked on problem definition, log standardization, model design, and the final presentation. The pipeline maps input columns and normalizes event types and timestamps into a common structure. The model combines event-and-time pretraining with two-stage fine-tuning based on BERT4Rec.

Evaluation achieved 79.85% masked-event reconstruction accuracy and a 91.53% purchase-timing hit rate within 24 hours. Purchase-classification precision remained an improvement target; notification fatigue and revenue impact require real-world validation.

</details>


### • Additional Projects

| Project | 내용 / Overview |
|:---|:---|
| [Nutrition Tracker OCR](https://github.com/Hyoju-1/nutrition_tracker_OCR) | OCR 모델을 활용한 영양정보 트래커 · Nutrition information tracker using OCR |

---

## 🔬 Research | 연구

### • B-MOD
**객체 크기에 따른 학습 편향을 줄이기 위한 손실함수 연구**

`Computer Vision` `Probabilistic Modeling` `Object Detection`

예측 영역과 정답 영역을 확률분포로 표현하고, 분포 간 유사도를 학습에 반영한 공동 연구입니다.

- **기여** — B-MOD 손실함수 제안 및 비교 실험
- **검증** — 신경망 구조를 유지한 상태에서 객체 크기 구성별 성능 비교
- **결과** — 소형·대형 객체 균형 조건의 평균 mAP@0.5 **0.629 → 0.685**
- **게재** — *Machine Vision and Applications*, 37, Article 42, 2026
- **저자 역할** — 공동 제1저자

[Paper →](https://doi.org/10.1007/s00138-026-01803-2) · [Code →](https://github.com/Hyoju-1/B-MOD_Yolov4)

<details>
<summary>English overview</summary>

Co-first-author research on a distribution-based loss for multi-scale object detection.

We evaluated loss-function changes while keeping the detector architecture fixed and compared performance across object-size distributions. Under the balanced small/large-object setting, mean mAP@0.5 improved from 0.629 with IoU to 0.685 with B-MOD.

Published in *Machine Vision and Applications* in 2026. The linked repository is a fork of the collaborative research repository.

</details>

### • Ontology-Guided Probing of VLM Evaluation
**비전·언어 모델의 평가 결과에 대한 진단 연구**

`Vision-Language Models` `Ontology` `Evaluation`

텍스트의 그럴듯함과 이미지에 근거한 정확성을 구분해 살펴보기 위한 평가 연구입니다. 온톨로지를 활용한 평가 코드와 통제 실험, 결과 요약 자료를 정리했습니다.

- **주요 내용** — 모델 간 비교, 평가 신호 분석, 교란 요인 통제 및 통계 검정
- **공개 자료** — 평가 스크립트, 요약 표, CSV·Markdown 결과 자료

[View repository →](https://github.com/Hyoju-1/Ontology-Guided-Probing-of-VLM-Evaluation)

<details>
<summary>English overview</summary>

Research on distinguishing textual plausibility from image-conditioned correctness in vision-language model evaluation.

The repository includes ontology-based evaluation code, cross-model comparisons, controlled diagnostic experiments, statistical tests, and selected result summaries.

</details>

### • IBP-based GC-MS Identification
**질량스펙트럼의 잠재 특징 학습과 물질 후보 검색**

`Bayesian Modeling` `Latent Features` `Scientific Data`

GC-MS 질량스펙트럼의 잠재 특징을 IBP로 학습하고, 재구성한 스펙트럼을 활용해 참조 라이브러리의 SMILES 후보를 검색·순위화합니다.

- **데이터 처리** — m/z·intensity 피크 정보의 행렬화 및 특징·가중치 구성
- **모델링** — 변분 IBP 기반 잠재 특징 학습과 스펙트럼 재구성
- **평가** — 재구성 품질과 후보 검색 성능을 구분해 Top-K·MRR·NDCG 등으로 확인

[View repository →](https://github.com/Hyoju-1/ibp-gcms-smiles)

<details>
<summary>English overview</summary>

A research pipeline that learns latent features from GC-MS mass spectra using a variational Indian Buffet Process.

Reconstructed spectra are used to retrieve and rank SMILES candidates from a reference library. The repository covers data preparation, latent-feature learning, reconstruction, and retrieval evaluation.

</details>

---

## Experience | 경험

### • Research & Coordination

| 영역 / Area | 경험 / Experience |
|:---|:---|
| **연구개발 과제 운영** | 연구실 내부 실무 담당자로서 제안서·계획서 작성, 진행 보고, 일정 및 협업 범위 조율 |
| **실험 설계와 검증** | 비교 조건 설정, 반복 실험, 성능과 적용 범위 분석 |
| **기술 소통** | 실험 목적·판단 근거·결과를 보고서와 발표 자료로 정리 |
| **협업 지원** | 데이터 통합 기준 제안, 구현 방법 및 주의점 문서화 |
| **자원 관리** | 과제별 예산과 집행 기한 통합 관리, 실행 가능한 대안 제안 |

<details>
<summary>English summary</summary>

<br>

- **R&D coordination:** Proposal and project-plan preparation, progress reporting, scheduling, and collaboration coordination within the lab.
- **Experimental evaluation:** Controlled comparisons, repeated experiments, and analysis of performance and applicability.
- **Technical communication:** Research reports and presentations explaining objectives, decisions, and results.
- **Team support:** Shared data definitions and implementation documentation.
- **Resource tracking:** Consolidated project budgets, spending deadlines, and actionable alternatives.

</details>

---

## Tools | 기술

| Area | Tools & Methods |
|:---|:---|
| **Programming & Data** | Python · pandas · NumPy · SciPy |
| **Machine Learning** | PyTorch · scikit-learn · Gaussian Processes · Uncertainty Evaluation |
| **LLM Applications** | RAG · Prompt Design · Gemini API · Upstage Solar · Local LLaMA · Pinecone |
| **Speech & Interfaces** | faster-whisper · Streamlit |
| **Vision & Multimodal** | YOLO · CLIP · OpenCLIP · SigLIP |
| **Scientific & Spatial Data** | RDKit · QGIS · Naver Maps API · T map API |
| **Documentation** | Jupyter · LaTeX · Research Reports · Presentations |

---

## 🎓 Background | 배경

| | |
|:---|:---|
| **Graduate Study** | Data Science, Inha University |
| **Undergraduate Major** | Statistics |
| **Additional Academic Background** | Business Administration |
| **Community** | BOAZ · Data Analysis |
| **Previous Work Experience** | Securities Settlement Operations |

경영·통계·AI를 공부하고 다양한 실무 환경을 경험하며, 기술과 업무를 함께 이해하는 시야를 넓혀가고 있습니다.

*Building an understanding of both technical methods and the work they support.*
