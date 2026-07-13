# ToBig's 26기 정규세션 — 통계적 추론과 회귀분석

데이터사이언스 학회 투빅스(TOBIGS) 26기 정규세션 **1주차 2교시: 통계적 추론과 회귀분석 (50분)** 자료 저장소입니다.
1교시(EDA·기술통계)에서 확인한 분포·상관·이상치를 바탕으로, 표본에서 관찰한 패턴이 모집단에서도 의미 있는지 판단하고(추론) 변수 간 관계를 회귀모델로 정량화하는 과정을 다룹니다.

## 구성

```
├── lecture/     # 발표자료 (발표자 노트 포함 PPT)
├── paper/       # 리뷰 논문 PDF + 선정 이유·요약
└── assignment/  # Colab 과제 + 모범답안
```

### 1. 강의자료 (`lecture/`)
- `발표자료_통계적추론과회귀분석.pptx` — 45슬라이드 50분 강의. **발표자 노트 포함** (각 슬라이드 노트에 강의 대사·배경설명 수록).
- 목차: EDA→추론 연결 / 통계적 추론 기본개념 / 표본분포·신뢰구간 / 가설검정 / 단순선형회귀 / 다중회귀 / 회귀 가정과 평가.
- **디자인**: 'AI 생성 티'가 나는 제목+불릿 획일 구조 대신 10종 레이아웃(statement·compare·figure·오해 callout·큰 숫자·steps 등)으로 구성. 근거·AI 티 체크리스트·참고자료는 [`lecture/발표자료_리디자인_노트.md`](lecture/발표자료_리디자인_노트.md).

### 2. 리뷰 논문 (`paper/`)
- **To Explain or to Predict?** — Galit Shmueli (Statistical Science (Institute of Mathematical Statistics), 2010). DOI: [10.1214/10-STS330](https://doi.org/10.1214/10-STS330)
- 선정 이유·한 문단 요약·DOI 출처는 [`paper/논문_선정이유_요약.md`](paper/논문_선정이유_요약.md) 참고.

### 3. Colab 과제 (`assignment/`)
- `assignment.ipynb` — 제출용 과제(빈칸/TODO 포함). Colab에서 열어 진행.
- `solution.ipynb` — 모범답안.
- 데이터: seaborn `tips` 데이터셋. 프로젝트형 흐름(로드→EDA→표본분포/CLT→신뢰구간→가설검정→단순/다중 회귀→진단→해석 vs 예측).
- 유형: A(기초 체화형) + B(도구 활용형). 마지막 셀에 생성형AI 활용 방법·대화 내역 기록.

## 과제 제출 방법
1. `assignment/assignment.ipynb`를 Colab에서 연다.
2. 각 셀의 TODO/빈칸을 채우고, 해석 질문(마크다운)에 직접 답한다.
3. 실험 결과·해석을 매주 기술블로그의 '과제 복습' 섹션과 연결해 정리한다.
4. 완성한 노트북을 제출한다.
