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
