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
- I-JEPA (2023, CVPR 2023) → JEPA World Model 계보
- V-JEPA (2024) → JEPA World Model 계보
- [ ] Var-JEPA (2026, ICML 2026) · arXiv:2603.20111
- [x] UWM-JEPA (2026) · arXiv:2605.25313 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2605.25313/)

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

## Self-Evolving Agent Skills 계보

에이전트의 모델 가중치는 고정하고, 스킬·프롬프트·문맥 같은 텍스트 상태를 경험으로 갱신해 성능을 올리는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 경험에서 배우는 언어 에이전트: 반성과 스킬 라이브러리
- [ ] Reflexion (2023, NeurIPS 2023) · arXiv:2303.11366
- [ ] Self-Refine (2023, NeurIPS 2023) · arXiv:2303.17651
- [ ] Voyager (2023, TMLR 2024) · arXiv:2305.16291

### 2. 텍스트 공간 최적화: LLM이 프롬프트와 파이프라인을 최적화
- [ ] OPRO (2023, ICLR 2024) · arXiv:2309.03409
- [ ] DSPy (2023, ICLR 2024) · arXiv:2310.03714
- [ ] TextGrad (2024, Nature 2025) · arXiv:2406.07496
- [x] GEPA (2025, ICLR 2026) · arXiv:2507.19457 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2507.19457/)

### 3. 에이전트 시스템과 문맥의 자동 진화
- [ ] ADAS (2024, ICLR 2025) · arXiv:2408.08435
- [ ] Agent Workflow Memory (2024, ICML 2025) · arXiv:2409.07429
- [ ] ACE: Agentic Context Engineering (2025, ICLR 2026) · arXiv:2510.04618
- [ ] EvoTest (2025, ICLR 2026) · arXiv:2510.13220

### 4. 에이전트 스킬의 정의와 평가
- [ ] SoK: Agentic Skills (2026) · arXiv:2602.20867
- [ ] SkillsBench (2026) · arXiv:2602.12670

### 5. 궤적 기반 스킬 구축과 진화
- [ ] Memp (2025, ACL 2026 Findings) · arXiv:2508.06433
- [ ] Trace2Skill (2026) · arXiv:2603.25158
- [ ] EvoSkill (2026) · arXiv:2603.02766
- [ ] CoEvoSkills (2026, COLM 2026) · arXiv:2604.01687
- [x] SkillOpt (2026) · arXiv:2605.23904 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2605.23904/)
- [x] Rethinking Self-Evolving Agents (OEO) (2026) · arXiv:2608.09629 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2608.09629/)

### 6. 강화학습과 결합한 스킬 학습
- [ ] SkillRL (2026) · arXiv:2602.08234
- [ ] Skill-Pro (2026, ICML 2026) · arXiv:2602.01869

## JEPA World Model 계보

픽셀을 복원하지 않고 latent 공간에서 미래 표현을 예측하는 JEPA를 행동 조건 세계 모델로 확장해,
latent 안에서 계획하고 불확실성을 다루는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. Latent 계획의 근본: 사전학습 특징 위의 세계 모델과 JEPA 계획
- [ ] DINO-WM (2024, ICML 2025) · arXiv:2411.04983
- [ ] PLDM: Planning with Latent Dynamics Models (2025) · arXiv:2502.14819
- [ ] V-JEPA 2 (2025) · arXiv:2506.09985
- [ ] What Drives Success in Physical Planning with JEPA World Models? (2025, TMLR) · arXiv:2512.24497

### 2. 픽셀에서 end-to-end로 안정 학습: 붕괴 없는 단일 목적 함수
- [ ] LeJEPA (2025) · arXiv:2511.08544
- [x] LeWorldModel (2026) · arXiv:2603.19312 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2603.19312/)
- [ ] UniJEPA (2026) · arXiv:2608.07409

### 3. 확률적·믿음 상태 JEPA: 미래 latent의 분포와 불확실성
- [ ] VJEPA: Variational JEPA as Probabilistic World Models (2026) · arXiv:2601.14354
- UWM-JEPA (2026) → Missing Modality Latent Prediction 계보
- [ ] Branch-JEPA: Finite-Support Predictive Distributions (2026) · arXiv:2607.05238

### 4. 행동 결합과 시험 시 적응: 예측기가 행동과 경험에 반응하게 만들기
- [ ] Delta-JEPA: Action-Sensitive World Models via Latent Difference Decoding (2026) · arXiv:2606.31232
- [ ] EPM-JEPA: Operator-Side Experience Modulation (2026) · arXiv:2606.12979

### 5. 이론: JEPA 세계 모델이 무엇을 배우는가
- [ ] When Does LeJEPA Learn a World Model? (2026) · arXiv:2605.26379
- [ ] A Generalization Theory for JEPA-Based World Models (2026) · arXiv:2606.27014
- [ ] UR-JEPA: Uniform Rectifiability as a Regularizer (2026) · arXiv:2606.01443

### 6. JEPA의 철학과 붕괴 방지: 픽셀 대신 표현을 예측하는 이유
- [ ] A Path Towards Autonomous Machine Intelligence (2022) · OpenReview BZ5a1r-kVsf
- [ ] I-JEPA (2023, CVPR 2023) · arXiv:2301.08243
- [ ] V-JEPA (2024) · arXiv:2404.08471
- [ ] V-JEPA 2.1: Unlocking Dense Features in Video Self-Supervised Learning (2026) · arXiv:2603.14482
- [ ] VICReg (2021, ICLR 2022) · arXiv:2105.04906

### 7. 재구성 기반 latent 월드 모델: latent 계획의 원형과 수술 적용
- [ ] PlaNet: Learning Latent Dynamics for Planning from Pixels (2018, ICML 2019) · arXiv:1811.04551
- [ ] DreamerV3 (2023, Nature 2025) · arXiv:2301.04104
- [ ] GAS: World Models for General Surgical Grasping (2024, RSS 2024) · arXiv:2405.17940 · 탭: Surgical WM
- [ ] Visuomotor Grasping with World Models for Surgical Robots (2025) · arXiv:2508.11200 · 탭: Surgical WM
- [ ] S2-HWM: Sparse Event-Structured Hierarchical World Model (2026) · arXiv:2608.13103 · 탭: Surgical WM

### 8. JEPA 인코더의 수술 도메인 사전학습
- [ ] OmniRAS: Standardizing Foundation Model Training and Evaluation in Robot-Assisted Surgery (2026) · arXiv:2608.31048

## Imitation Gap 계보

훈련 때만 쓸 수 있는 특권 정보(privileged information)를 가진 교사를 부분 관측 학생이
모방할 때 생기는 imitation gap을 정의하고, 모방과 강화학습을 섞거나 교사를 학생에 맞춰
학습해 그 간극을 메우는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 특권 정보 활용의 근본: 비대칭 critic과 특권 교사 모방
- [ ] Asymmetric Actor Critic for Image-Based Robot Learning (2017) · arXiv:1710.06542
- [ ] Learning by Cheating (2019, CoRL 2019) · arXiv:1912.12294
- [ ] Privileged Information Dropout in RL (2020) · arXiv:2005.09220

### 2. Imitation gap의 정의와 모방·RL의 적응적 전환
- [x] ADVISOR: Bridging the Imitation Gap by Adaptive Insubordination (2020, NeurIPS 2021) · arXiv:2007.12173 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2007.12173/)
- [ ] A2D: Robust Asymmetric Learning in POMDPs (2020, ICML 2021) · arXiv:2012.15566
- [ ] COSIL: Leveraging Fully Observable Policies for Learning under Partial Observability (2022, CoRL 2022) · arXiv:2211.01991
- [ ] Impossibly Good Experts and How to Follow Them (2023, ICLR 2023) · OpenReview sciA_xgYofB
- [ ] TGRL: Teacher Guided Reinforcement Learning (2023, ICML 2023) · arXiv:2307.03186

### 3. 학생을 고려한 교사 학습: 교사와 학생의 공동 학습, 학생 중심 전문가 설계
- [ ] SITT: Student-Informed Teacher Training (2024, ICLR 2025) · arXiv:2412.09149
- [ ] GPO: Guided Policy Optimization under Partial Observability (2025, ICLR 2026) · arXiv:2505.15418
- [ ] LEAD: Minimizing Learner-Expert Asymmetry in End-to-End Driving (2025, CVPR 2026) · arXiv:2512.20563
- [ ] Teacher-Student Representational Alignment for RL-Driven Imitation Learning (2026, ICRA 2026 RL4IL Workshop) · arXiv:2605.28372

### 4. 불확실성과 사전 정보로 간극 메우기
- [ ] BIG: A Bayesian Solution To The Imitation Gap (2024, NeurIPS 2024) · arXiv:2407.00495
- [ ] IGDrivSim: A Benchmark for the Imitation Gap in Autonomous Driving (2024) · arXiv:2411.04653

### 5. 비대칭 RL의 이론과 확장: 특권 critic·모델·센서
- [ ] Unbiased Asymmetric RL under Partial Observability (2021, AAMAS 2022) · arXiv:2105.11674
- [ ] Learning in POMDPs is Sample-Efficient with Hindsight Observability (2023, ICML 2023) · arXiv:2301.13857
- [ ] Scaffolder: Privileged Sensing Scaffolds RL (2024, ICLR 2024) · arXiv:2405.14853
- [ ] Provable Partially Observable RL with Privileged Information (2024, NeurIPS 2024) · arXiv:2412.00985
- [ ] PIGDreamer: Privileged Information Guided World Models (2025) · arXiv:2508.02159
- [ ] Informed Asymmetric Actor-Critic (2025) · arXiv:2509.26000

### 6. 언제 증류하고 언제 직접 배우는가
- [ ] To Distill or Decide? (2025, NeurIPS 2025) · arXiv:2510.03207

## Trajectory Long-Tail 계보

자율주행 궤적 예측(trajectory prediction)에서 드물지만 위험한 long-tail 장면을 정의하고,
상호작용 구조를 모델링하거나 학습 데이터를 고르고 늘려 그 장면에서의 예측을 개선하는 연구 흐름.
리뷰 순서는 위에서 아래로, 우선순위가 높은 논문을 각 갈래 앞에 두었다.

### 1. Data-centric: 학습 데이터를 고르거나 늘려서 tail 대응
- [x] Den-TP (2024, CVPR 2026) · arXiv:2409.17385 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2409.17385/)
- [ ] GALTraj (2025, ICCV 2025) · arXiv:2507.22615
- [ ] Critical Example Mining with Flow-based Generative Models (2024) · arXiv:2410.16083
- [ ] Trajectory Entropy Maximization Data Pruning (2025) · arXiv:2512.19270

### 2. 명시적 상호작용 구조: 상호작용 그래프와 조건부 분해
- [ ] FJMP (2022, CVPR 2023) · arXiv:2211.16197
- [ ] M2I (2022, CVPR 2022) · arXiv:2202.11884
- [ ] GameFormer (2023, ICCV 2023) · arXiv:2303.05760
- [ ] Density-Adaptive Model Based on Motif Matrix (2024, CVPR 2024) · CVF Open Access
- [ ] Super Agents and Confounders (2026) · arXiv:2604.03463

### 3. Long-tail 정의와 표현 학습: 어려운 샘플을 가르고 따로 배우기
- [ ] AMD (2025, ICCV 2025) · arXiv:2507.01801
- [ ] On Exposing the Challenging Long Tail in Future Prediction of Traffic Actors (2021, ICCV 2021) · arXiv:2103.12474
- [ ] FEND (2023, CVPR 2023) · arXiv:2303.16574
- [ ] TrACT (2024, IV 2024) · arXiv:2404.12538
- [ ] SAML: Differentiable Semantic Meta-Learning (2025, AAAI 2026) · arXiv:2511.06649
- [ ] SAIL (2026) · arXiv:2604.04573

### 4. 기준 모델과 데이터셋
- [ ] QCNet: Query-Centric Trajectory Prediction (2023, CVPR 2023) · CVF Open Access
- [ ] Argoverse 2 (2023, NeurIPS 2021 Datasets and Benchmarks) · arXiv:2301.00493

## Driving VLA 계보

카메라 영상과 언어를 함께 다루는 VLM을 주행 정책에 결합해, 장면을 말로 설명하는 단계에서
궤적을 직접 출력하고 그 전에 추론하는 단계까지 발전한 연구 흐름.
갈래는 VLA4AD 서베이(arXiv:2506.24044)의 발전 단계를 따르고, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. End-to-end 주행의 근본: 인식에서 계획까지 하나의 네트워크로
- [ ] UniAD (2022, CVPR 2023) · arXiv:2212.10156
- [ ] VAD (2023, ICCV 2023) · arXiv:2303.12077

### 2. 설명자로서의 언어 모델: 장면과 판단을 말로 설명
- [ ] DriveGPT4 (2023, RA-L) · arXiv:2310.01412
- [ ] DriveLM (2023, ECCV 2024) · arXiv:2312.14150
- [ ] GPT-Driver (2023) · arXiv:2310.01415
- [ ] RAG-Driver (2024, RSS 2024) · arXiv:2402.10828

### 3. 모듈형·이중 시스템 VLA: VLM의 판단을 planner가 궤적으로 변환
- [ ] DriveVLM (2024, CoRL 2024) · arXiv:2402.12289
- [ ] Senna (2024, IJCV) · arXiv:2410.22313
- [ ] OpenDriveVLA (2025, AAAI 2026) · arXiv:2503.23463

### 4. 통합 end-to-end VLA: 센서에서 궤적까지 하나의 모델
- [ ] LMDrive (2023, CVPR 2024) · arXiv:2312.07488
- [ ] EMMA (2024, TMLR) · arXiv:2410.23262
- [ ] SimLingo (2025, CVPR 2025) · arXiv:2503.09594
- [ ] NoRD: Drives without Reasoning (2026, CVPR 2026) · arXiv:2602.21172

### 5. 추론 강화 VLA: CoT와 강화학습으로 행동 전에 추론
- [ ] ORION (2025, ICCV 2025) · arXiv:2503.19755
- [ ] AutoVLA (2025, NeurIPS 2025) · arXiv:2506.13757
- [ ] Impromptu VLA (2025, NeurIPS 2025) · arXiv:2505.23757
- [ ] ReCogDrive (2025) · arXiv:2506.08052
- [ ] Alpamayo-R1 (2025) · arXiv:2511.00088

### 6. 행동에 근거한 추론과 월드 모델: 텍스트 대신 미래 장면·잠재 표현으로 추론
- [ ] FutureSightDrive (2025, NeurIPS 2025) · arXiv:2505.17685
- [ ] IRL-VLA (2025) · arXiv:2508.06571
- [ ] DriveVLA-W0 (2025) · arXiv:2510.12796
- [ ] DriveWorld-VLA (2026) · arXiv:2602.06521
- [ ] LaST-VLA (2026) · arXiv:2603.01928

### 7. 평가 벤치마크
- [ ] NAVSIM (2024, NeurIPS 2024 D&B) · arXiv:2406.15349
- [ ] Bench2Drive (2024, NeurIPS 2024 D&B) · arXiv:2406.03877
- [ ] Pseudo-Simulation (NAVSIM v2) (2025, CoRL 2025) · arXiv:2506.04218
- [ ] WOD-E2E (2025) · arXiv:2510.26125

### 참고 서베이 (리뷰 대상 아님)
- End-to-end Autonomous Driving: Challenges and Frontiers (2023, TPAMI) · arXiv:2306.16927
- A Survey on VLA Models for Autonomous Driving (2025, ICCV 2025 Workshops) · arXiv:2506.24044
- VLA Models for Autonomous Driving: Past, Present, and Future (2025) · arXiv:2512.16760
- A Survey of World Models for Autonomous Driving (2025) · arXiv:2501.11260
- Beyond Textual Chain-of-Thought (2026, EMNLP 2026) · arXiv:2609.01659

## Surgical Robot Safety 계보

수술 로봇의 모방학습 정책이 실행 중에 실패하는 순간을 감지하고, 월드 모델과 시뮬레이터로 정책을 학습·평가해
수술 자율화의 안전성을 확보하는 연구 흐름.
리뷰 순서는 위에서 아래로, 우선순위가 높은 논문을 각 갈래 앞에 두었다.

### 1. 실행 중 실패 감지: 정책이 실패하는 순간을 잡아냄
- [x] FoMo-FD: Failure Detection for Surgical Robot Imitation Policies via Flow-Matching World Modeling (2026) · arXiv:2607.27511 · 탭: Surgical WM · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2607.27511/)
- [x] FARM: Reading Failure Signals from the Internal Predictive States of a Frozen Robotic World Model (2026) · arXiv:2609.11445 · [리뷰](https://hyunjikim12.github.io/paper-review/posts/2609.11445/)
- [ ] SAFE: Multitask Failure Detection for Vision-Language-Action Models (2025, NeurIPS 2025) · arXiv:2506.09937
- [ ] FIPER: Failure Prediction at Runtime for Generative Robot Policies (2025, NeurIPS 2025) · arXiv:2510.09459
- [ ] Foundational World Models Accurately Detect Bimanual Manipulator Failures (2026, ICRA 2026) · arXiv:2603.06987
- [ ] FAIL-Detect: Can We Detect Failures Without Failure Data? (2025, RSS 2025) · arXiv:2503.08558
- [ ] Sentinel: Unpacking Failure Modes of Generative Policies (2024, CoRL 2024) · arXiv:2410.04640
- [ ] RC-NF (2026, CVPR 2026) · arXiv:2603.11106
- [ ] Early Failure Detection in Autonomous Surgical Soft-Tissue Manipulation via Uncertainty Quantification (2025, RSS 2025 Workshop) · arXiv:2501.10561
- [ ] FailSafe: Reasoning and Recovery from Failures in VLA Models (2025, IROS 2026) · arXiv:2510.01642
- [ ] FailBench: How Reliable are VLMs at Judging Robot Task Success? (2026) · arXiv:2609.03611

### 2. 수술 안전 감지와 오류 검출
- [ ] Real-Time Context-Aware Detection of Unsafe Events in Robot-Assisted Surgery (2020, DSN 2020) · arXiv:2005.03611
- [ ] Runtime Detection of Executional Errors in Robot-Assisted Surgery (2022, ICRA 2022) · arXiv:2203.00737
- [ ] SEDCLIP: Adapting VLM for Multi-Label Surgical Error Detection (2026, Medical Image Analysis 2026) · DOI 10.1016/j.media.2026.104276

### 3. 수술 로봇 모방학습, 시뮬레이션, 플랫폼
- [ ] ORBIT-Surgical (2024, ICRA 2024) · arXiv:2404.16027
- [ ] SRT: Surgical Robot Transformer (2024, CoRL 2024) · arXiv:2407.12998
- [ ] Imitation Learning for Robot Assistance in Open Surgery: A Multi-Policy Evaluation on Suture Following (2026) · arXiv:2605.28736
- [ ] FF-SRL (2025, IROS 2024) · arXiv:2503.18616
- [ ] SurRoL (2021, IROS 2021) · arXiv:2108.13035
- [ ] Supervised Mixture-of-Experts for Surgical Grasping and Retraction (MoE-ACT) (2026, RSS 2026) · arXiv:2601.21971
- [ ] Surgical Embodied Intelligence for Generalized Task Autonomy in Laparoscopic RAS (2025, Science Robotics 2025) · DOI 10.1126/scirobotics.adt3093
- [ ] SRT-H (2025, Science Robotics 2025) · arXiv:2505.10251
- [ ] LapGym (2023, JMLR 2023) · arXiv:2302.09606
- [ ] SutureBot (2025, NeurIPS 2025) · arXiv:2510.20965
- [ ] SurgVIL: Scaling Surgical Robot Imitation Learning with Open-source Surgical Videos (2026) · arXiv:2608.16058
- [ ] dVRK: An Open-Source Research Kit for the da Vinci Surgical System (2014, ICRA 2014) · DOI 10.1109/ICRA.2014.6907809
- [ ] JIGSAWS: JHU-ISI Gesture and Skill Assessment Working Set (2014, MICCAI 2014 M2CAI Workshop)

### 4. 일반 로봇 정책 배경
- [ ] ACT/ALOHA: Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware (2023, RSS 2023) · arXiv:2304.13705
- [ ] Diffusion Policy (2023, RSS 2023) · arXiv:2303.04137
- [ ] SmolVLA (2025) · arXiv:2506.01844

### 5. 월드 모델 기반 정책 평가
- [ ] Cosmos-Surg-dVRK (2025, RA-L 2025) · arXiv:2510.16240 · 탭: Surgical WM
- [ ] SurgWMBench (2026) · arXiv:2608.08070 · 탭: Surgical WM
- [ ] Ctrl-World (2025, ICLR 2026) · arXiv:2510.10125
- [ ] WorldGym (2025, ICLR 2026) · arXiv:2506.00613
- [ ] Open-H-Embodiment (2026) · arXiv:2604.21017
- [ ] RoboWM-Bench (2026, CVPR 2026 Workshop) · arXiv:2604.19092
- [ ] UniSim: Learning Interactive Real-World Simulators (2023, ICLR 2024) · arXiv:2310.06114
- [ ] WorldEval (2025) · arXiv:2505.19017

- 생성형 수술 월드 모델 (Surgical Vision World Model, Cosmos-H-Surgical, SurgVista, Cosmos-H-Dreams, KVLR) → World-Action Model 계보

### 6. 분야 관점
- [ ] A Decade Retrospective of Medical Robotics Research from 2010 to 2020 (2021, Science Robotics 2021) · DOI 10.1126/scirobotics.abi8017
- [ ] General-Purpose Foundation Models for Increased Autonomy in Robot-Assisted Surgery (2024, Nature Machine Intelligence 2024) · arXiv:2401.00678

## Surgical Video VLM 계보

수술·의료 영상을 이해하는 VLM을 GRPO 같은 강화학습으로 학습하고, 수술 영상 이해의 과제와 데이터를 정리하는 연구 흐름.
리뷰 순서는 위에서 아래로, 우선순위가 높은 논문을 각 갈래 앞에 두었다.

### 1. 강화학습으로 학습하는 의료·수술 영상 VLM
- [ ] MedGRPO (2025, CVPR 2026) · arXiv:2512.06581
- [ ] Surgery-R1 (2025) · arXiv:2506.19469
- [ ] Video-R1 (2025, NeurIPS 2025) · arXiv:2503.21776

### 2. GRPO와 검증 가능한 보상 기반 RL
- [ ] DeepSeekMath (2024) · arXiv:2402.03300
- [ ] DeepSeek-R1 (2025, Nature 2025) · arXiv:2501.12948
- [ ] DAPO (2025) · arXiv:2503.14476

### 3. 수술 영상 이해의 과제와 데이터
- [ ] Rendezvous (2021, Medical Image Analysis 2022) · arXiv:2109.03223
- [ ] CholecTriplet2021 (2022, Medical Image Analysis 2023) · arXiv:2204.04746
- [ ] SurgPub-Video (2025, AAAI 2026) · arXiv:2508.10054
- [ ] SurgGraph (2026) · arXiv:2609.25651
- [ ] SurgVLP (2023, Medical Image Analysis 2025) · arXiv:2307.15220
- [ ] SurgVISTA: Large-scale Self-supervised Video Foundation Model for Intelligent Surgery (2025, npj Digital Medicine 2026) · arXiv:2506.02692
- [ ] Surg-3M / SurgFM: A Dataset and Foundation Model for Perception in Surgical Settings (2025) · arXiv:2503.19740
- [ ] Surgical-VQA (2022, MICCAI 2022) · arXiv:2206.11053

## World-Action Model 계보

미래 관측(영상)과 실행 가능한 행동을 하나의 생성 모델이 함께 예측하거나, 행동을 조건으로 미래 영상을 생성해
정책·월드 모델·시뮬레이터 역할을 한 모델로 통합하는 연구 흐름.
리뷰 순서는 위에서 아래로, 갈래별로 근본 논문 → 파생 논문 순이다.

### 1. 근본: 영상 예측과 행동 생성의 통합
- [ ] Unified Video Action Model (UVA) (2025) · arXiv:2503.00200
- [ ] Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning (2026) · arXiv:2601.16163
- [ ] LingBot-VA: Causal World Modeling for Robot Control (2026, RSS 2026) · arXiv:2601.21998

### 2. 행동 조건 영상 생성: 행동을 입력받아 미래 수술 영상을 생성해 정책 학습·시뮬레이션에 활용
- [ ] Surgical Vision World Model (2025, MICCAI 2025 Workshop) · arXiv:2503.02904 · 탭: Surgical WM
- [ ] Cosmos-H-Surgical (SurgWorld) (2025) · arXiv:2512.23162 · 탭: Surgical WM
- [ ] KVLR: From Articulated Kinematics to Routed Visual Control for Action-Conditioned Surgical Video Generation (2026, NeurIPS 2026) · arXiv:2605.08712 · 탭: Surgical WM
- [ ] SurgVista: Long-Horizon Surgical World Modeling (2026) · arXiv:2606.19889 · 탭: Surgical WM
- [ ] Cosmos-H-Dreams (2026) · arXiv:2608.24199 · 탭: Surgical WM

### 3. 수술 WAM: 내시경 영상과 수술 로봇 행동의 공동 예측
- [ ] Surgical WAM: A World-Action Model for Data-Efficient Surgical Robot Learning (2026) · arXiv:2608.11204 · 탭: Surgical WM
- [ ] Towards Surgical World-Action Modeling (2026) · arXiv:2608.20284 · 탭: Surgical WM
- [ ] EndoWAM: A Grounded World-Action Model for Generalizable Endoscopic Navigation (2026) · arXiv:2608.01221 · 탭: Surgical WM
