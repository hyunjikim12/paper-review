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
