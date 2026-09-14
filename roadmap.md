# 논문 리뷰 로드맵

## Pathology Agent 계보

병리 전체 슬라이드 이미지(WSI)를 LLM/MLLM 에이전트가 탐색·추론하는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. Training-free 탐색형: 학습 없이 기존 모델을 조율해 추론
- [x] PathAgent (2025, ECCV 2026) · arXiv:2511.17052 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2511.17052/)
- [ ] GIANT (2025) · arXiv:2511.19652
- [ ] PathNavigate (2026) · arXiv:2605.23559
- [ ] BEACON (2026) · arXiv:2608.05757
- [ ] AdaptivePath (2026) · arXiv:2608.08648

### 2. 멀티에이전트 협업형: 역할을 나눈 에이전트들이 슬라이드를 함께 분석
- [ ] PathFinder (2025) · arXiv:2502.08916
- [ ] SlideSeek (2025) · arXiv:2506.20964
- [ ] WSI-Agents (2025) · arXiv:2507.14680

### 3. 학습 기반 탐색형: 병리의의 슬라이드 탐색 방식을 모델에 학습
- [ ] CPathAgent (2025) · arXiv:2505.20510
- [ ] Pathology-CoT (2025) · arXiv:2510.04587
- [ ] PathFound (2025) · arXiv:2512.23545
- [ ] MMNavAgent (2026) · arXiv:2603.02079

### 4. 도구·지식 확장형: 검색(RAG), 도구 생성, 과거 사례 활용
- [ ] Patho-AgenticRAG (2025) · arXiv:2508.02258
- [ ] TissueLab (2025) · arXiv:2509.20279
- [ ] SurvAgent (2025) · arXiv:2511.16635
- [ ] PathoSage (2026) · arXiv:2606.07549

## Latent Multi-Agent 계보

LLM 에이전트들이 텍스트 대신 hidden state·KV cache 같은 잠재 표현으로 추론하고 협업하는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 잠재 공간 협업 MAS: 텍스트 대신 hidden state·KV cache로 협업
- [x] LatentMAS (2025, ICML 2026) · arXiv:2511.20639 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2511.20639/)
- [ ] Recursive Multi-Agent Systems (2026) · arXiv:2604.25917
- [ ] Cache Merging as a Convergent Replicated State for Multi-Agent Latent Reasoning (2026) · arXiv:2607.01308

### 2. 이종·비전 모델로의 확장: VLM 시각 입력 경로를 잠재 통신 채널로 활용
- [x] The Vision Wormhole (2026) · arXiv:2602.15382 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2602.15382/)
- [ ] Post-Hoc Sparse Coding of Latent Communication Between Vision-Language Model Agents (2026) · arXiv:2608.10198

### 3. 잠재 메모리: 에이전트별 경험을 압축된 잠재 표현으로 저장
- [ ] LatentMem (2026) · arXiv:2602.03036

### 4. 에이전트 간 잠재 통신: 임베딩·활성값·KV cache 전달
- [ ] CIPHER: Let Models Speak Ciphers (2023) · arXiv:2310.06272
- [ ] Communicating Activations Between Language Model Agents (2025) · arXiv:2501.14082
- [ ] KVComm (2025) · arXiv:2510.03346
- [ ] Cache-to-Cache (2025) · arXiv:2510.03215
- [ ] Thought Communication in Multiagent Collaboration (2025) · arXiv:2510.20733
- [ ] Interlat: Enabling Agents to Communicate Entirely in Latent Space (2025) · arXiv:2511.09149

### 5. 단일 모델 잠재 추론
- [ ] Coconut: Training LLMs to Reason in a Continuous Latent Space (2024) · arXiv:2412.06769

### 6. 텍스트 기반 MAS
- [ ] Multiagent Debate (2023) · arXiv:2305.14325
- [ ] Chain of Agents (2024) · arXiv:2406.02818

### 7. 잠재 통신의 안전성
- [ ] LCGuard (2026) · arXiv:2605.22786
- [ ] When Latent Agents Lie: KV-Cache Integrity (2026) · arXiv:2606.28958

## Visual Token Pruning 계보

MLLM/VLM에 들어가는 많은 시각 토큰 중 일부만 남겨 추론 비용을 줄이는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 어텐션 기반 중요도 선택: 어텐션 점수로 남길 토큰을 고름
- [x] FastV (2024, ECCV 2024) · arXiv:2403.06764 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2403.06764/)
- [ ] SparseVLM (2024, ICML 2025) · arXiv:2410.04417
- [ ] VisionZip (2024, CVPR 2025) · arXiv:2412.04467

### 2. 다양성·커버리지 기반 선택: 전체를 대표하는 토큰 부분집합 구성
- [x] DivPrune (2025, CVPR 2025) · arXiv:2503.02175 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2503.02175/)
- [ ] SCOPE (2025, NeurIPS 2025) · arXiv:2510.24214
- [ ] MMTok (2025, ICLR 2026) · arXiv:2508.18264
- [ ] EVTP-IVS (2025, WACV 2026) · arXiv:2508.11886
- [ ] SCoRe (2026, CVPR 2026) · CVF Open Access
- [ ] TOPS (2026) · arXiv:2606.27161

### 3. Pruning 실패 분석: 어떤 과제에서 왜 무너지는가
- [x] Why and When Visual Token Pruning Fails? (2026, ECCV 2026) · arXiv:2604.12358 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2604.12358/)

### 4. KV cache 압축: 캐시 단계에서 시각 토큰 줄이기
- [ ] VL-Cache (2024, ICLR 2025) · arXiv:2410.23317

## Medical VLM Hallucination 계보

의료 VLM이 이미지 근거 없이 그럴듯한 답이나 판독문을 만들어 내는 환각(hallucination)을 측정·탐지·완화하는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 평가·벤치마크: 의료 VLM 환각을 정의하고 측정
- [ ] Med-HallMark (2024) · arXiv:2406.10185
- [ ] ProbMed: Worse than Random? (2024, ACL 2025 Findings) · arXiv:2405.20421
- [ ] MedHEval (2025) · arXiv:2503.02157
- [ ] HEAL-MedVQA / LobA (2025, IJCAI 2025) · arXiv:2505.00744

### 2. 환각 탐지: 불확실성·검증으로 환각 응답을 걸러냄
- [ ] RadFlag (2024, ML4H 2024) · arXiv:2411.00299
- [ ] VASE (2025, MICCAI 2025) · arXiv:2503.20504
- [ ] VIHD (2026, MICCAI 2026) · arXiv:2605.20772
- [ ] CoEV (2026, MICCAI 2026) · arXiv:2606.18609

### 3. 학습 없는 디코딩 개입: 추론 시 시각 근거 쪽으로 출력을 교정
- [ ] VCD (2023, CVPR 2024) · arXiv:2311.16922
- [ ] Prompt Highlighter (2023, CVPR 2024) · arXiv:2312.04302
- [ ] Expert-CFG (2025, ICCV 2025) · arXiv:2507.09209
- [ ] CCD (2025, ACL 2026 Findings) · arXiv:2509.23379
- [ ] Med-VCD (2025, Computers in Biology and Medicine 2026) · arXiv:2512.01922
- [x] ARCD (2025, AAAI 2026) · arXiv:2512.17189 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2512.17189/)
- [ ] CAST (2026, MICCAI 2026) · arXiv:2608.17427

### 4. 검색 증강(RAG): 외부 지식으로 사실성 보강
- [ ] RULE (2024, EMNLP 2024) · arXiv:2407.05131
- [ ] FactMM-RAG (2024, NAACL 2025) · arXiv:2407.15268
- [ ] MMed-RAG (2024, ICLR 2025) · arXiv:2410.13085
- [ ] HeteroRAG (2025, ACL 2026 Findings) · arXiv:2508.12778

### 5. 선호 최적화·강화학습: 환각 응답을 덜 선호하도록 정렬
- [ ] DPO for Suppressing Hallucinated Prior Exams (2024, MLHC 2024) · arXiv:2406.06496
- [ ] MMedPO (2024, ICML 2025) · arXiv:2412.06141
- [ ] CheXalign (2024, ACL 2025) · arXiv:2410.07025
- [ ] Benchmarking DPO for Medical LVLMs (2026, EACL 2026 Findings) · arXiv:2601.17918

### 6. 시각 근거 기반 생성·교정: 소견을 이미지 영역에 연결
- [ ] MAIRA-2 (2024) · arXiv:2406.04449
- [ ] FactCheXcker (2024, CVPR 2025) · arXiv:2411.18672
- [ ] Phrase-grounded Fact-checking for Chest X-ray Reports (2025, MICCAI 2025) · arXiv:2509.21356

### 7. 멀티에이전트 검증: 에이전트 간 반박·검증으로 진단 환각 억제
- [ ] MedMMV (2025) · arXiv:2509.24314
- [ ] Dialectic-Med (2026, ACL 2026 Findings) · arXiv:2604.11258

## Missing Modality Latent Prediction 계보

빠진 모달리티나 문맥을 입력 공간이 아니라 latent 공간에서 예측하고, 그 예측의 불확실성까지 다루는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. JEPA 근본: 입력 대신 latent를 예측
- [ ] I-JEPA (2023, CVPR 2023) · arXiv:2301.08243
- [ ] V-JEPA (2024) · arXiv:2404.08471
- [ ] Var-JEPA (2026, ICML 2026) · arXiv:2603.20111

### 2. Missing modality 기초: 빠진 모달리티의 복원과 우회
- [ ] SMIL (2021, AAAI 2021) · arXiv:2103.05677
- [ ] ShaSpec (2023, CVPR 2023) · arXiv:2307.14126
- [ ] Deep Multimodal Learning with Missing Modality: A Survey (2024, TMLR) · arXiv:2409.07825

### 3. 추론 가능한 정보와 고유 정보의 구분
- [x] MUST (2026, CVPR 2026) · arXiv:2603.26071 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2603.26071/)

### 4. Embedding 공간에서의 missing latent 예측
- [ ] Missing Modality Prediction via Joint Embedding of Unimodal Models (2024, ECCV 2024) · arXiv:2407.12616
- [x] ProM3E (2025, CVPR 2026) · arXiv:2511.02946 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2511.02946/)
- [ ] Mol-JEPA (2026) · arXiv:2608.22642

### 5. 불확실성을 판단과 정렬에 활용
- [ ] CalMRL (2025, ICML 2026) · arXiv:2511.12034
- [ ] EASE (2026, ACL 2026 Findings) · ACL Anthology 2026.findings-acl.260
