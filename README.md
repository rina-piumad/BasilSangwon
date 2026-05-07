## 정상원 · Basil Sangwon Jung

> **On-Premise RAG / Document AI Engineer** · 11년차 시스템 SW 엔지니어
RAG / Document AI 쪽 일을 하고 있습니다.
---

### 지금 하고 있는 일

**On-Premise Hybrid RAG (Phase 1 → 3)**
폐쇄망에서 BM25 + Vector(pgvector / ChromaDB) + Graph(Neo4j) 3-way Retrieval.
3-hop 한계 확인 후 재랭킹·청크 재설계·KG 도입 3안을 비교, Neo4j 결합으로 5홉 추론까지 확장.
LLM-as-a-Judge로 결정 사후 검증

**RAG Document Parser (Vision OCR)**
Qwen3.5-35B Vision OCR + EasyOCR 교차 검증 + Diff Engine + glossary 기반 오인식 교정.
1,000페이지+ 한글 PDF의 표·도형·컬럼 레이아웃 구조화.
**88페이지 25분 → 5분 (5배), 타임아웃 복구율 98%+**.

**USPTO 특허 승인 예측 — QLoRA Fine-tuning** *(개인 연구)*
Qwen3.5-9B를 DGX Spark 128GB 단일 머신에서 안정 학습 완주.
NF4 4-bit Double Quant + LoRA(MLP 확장) + cosine LR + EarlyStopping +
resume-constant-LR 4대 의사결정으로 하드웨어 증설 없이 9B 학습.
USPTO 725만 페어, **Pilot Loss 4.57 → 0.44 (-90.4%), Eval Accuracy 46.4% → 60.8%**.

---

### 공개된 저장소

회사 프로젝트 위주라 Public 코드는 적습니다. RAG 핵심 아이디어는 아래 두 곳에서 볼 수 있습니다.

| 저장소 | 한 줄 설명 |
|---|---|
| **[Hybrid-RAG-Chatbot](https://github.com/BasilSangwon/Hybrid-RAG-Chatbot)** | BM25 + ChromaDB + Neo4j RRF 융합, LangChain NL→Cypher, Semantic Cache, 9개 모델 비교 |
| **[Multi-hop-Knowledge-Graph-Chatbot](https://github.com/BasilSangwon/Multi-hop-Knowledge-Graph-Chatbot)** | 3-way Hybrid RAG + Knowledge Graph 멀티홉 추론 실험 |
| **[WebScrapingWpf](https://github.com/BasilSangwon/WebScrapingWpf)** | C# WPF 개인용 스크래핑 툴 |

상세 구조·의사결정 로그는 Notion 정리본으로 대체합니다.

- [Secure On-Premise AI Chatbot](https://flax-receipt-b4c.notion.site/Secure-On-Premise-AI-Chatbot-2c35cbfd76968020bf5cc8b8dd2d07ab) — 폐쇄망 vLLM 기반 Local LLM 서빙
- [RAG Document Parser](https://flax-receipt-b4c.notion.site/RAG-Document-Parser-3135cbfd76968028aa0df1dfced7c35d) — Vision OCR 파이프라인 + 교차 검증
- [USPTO QLoRA Fine-tuning](https://flax-receipt-b4c.notion.site/USPTO-AI-3185cbfd76968038ab08db5ce82dac65) — 9B 단일 머신 학습 회고
- [Samsung Whiteboard](https://flax-receipt-b4c.notion.site/Samsung-Whiteboard-656d087ea1e44dbbb1033b4a534c0caf) — 11개 언어 글로벌 B2B 런칭
- [WireScreen](https://flax-receipt-b4c.notion.site/WireScreen-2d15cbfd769680539927c0d4a4a01062) — DXGI + NVENC GPU Zero-Copy, End-to-End 24ms

---

### 주로 쓰는 것

| 영역 | 스택 |
|---|---|
| **LLM / Fine-tuning** | Python · PyTorch · Hugging Face (peft, bitsandbytes, transformers) · QLoRA · NF4 · vLLM · LangChain |
| **RAG / Retrieval** | pgvector · FAISS · BM25 · Neo4j · ChromaDB · BGE-M3 · Cross-Encoder · RRF Fusion · Cypher |
| **Vision / Speech** | YOLOv8 · Qwen-VL · EasyOCR · pypdfium2 · Faster-Whisper · Pyannote · ECAPA-TDNN |
| **Backend / Infra** | FastAPI · PostgreSQL · Docker · CUDA · DGX Spark (GB10) · Synology NAS |
| **Legacy (11년 자산)** | C# · .NET WPF · Win32 API (Raw Input / HID / DXGI) · NVENC · D3D11 · WebRTC · FFmpeg |

---

### 경력

| 기간 | 회사 | 역할 |
|---|---|---|
| 2022.04 – 현재 | **㈜테크에이스지엑스** *(삼성전자 B2B 전자칠판 공식 협력사)* | Technical Lead |
| 2020.08 – 2021.12 | ㈜아이엠파인 | System Software Engineer |
| 2015.09 – 2020.08 | ㈜이노시뮬레이션 *(방산·가상훈련)* | Tool Development Lead |
| 2015.03 – 2015.08 | 용현시스템 | Core Client Developer |

총 11년 · 학점은행제 컴퓨터공학 4년제 졸업 (직장 병행 야간·주말 이수)

---

basilsangwon@naver.com · 경기 화성
