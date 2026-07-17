# 통계적 추론과 회귀분석 · ToBig's 26기 정규세션

> **표본에서 모집단으로 — 통계적 추론과 회귀분석** (1주차 2교시)
> 데이터사이언스 학회 **투빅스(ToBig's) 26기** 정규세션 자료 저장소입니다.

**Framingham 심장연구** 데이터 하나로 **EDA → 통계적 추론 → 회귀 → 예측**을 처음부터 끝까지 관통합니다.
발표자료(발표자 노트 포함)·리뷰 논문·Colab 과제(모범답안 포함)를 담았습니다.

```
📂 repo
├── lecture/      발표자료 (.pptx, 발표자 노트 포함) + .pdf
├── paper/        리뷰 논문 PDF + 선정 이유·요약
└── assignment/   Colab 과제 + 모범답안 + 데이터
```

---

## 🎬 강의자료 · `lecture/`

- `발표자료_통계적추론과회귀분석.pptx` — **86슬라이드**, 각 슬라이드 노트에 강의 대사·배경설명 수록. 뷰어용 **PDF** 동봉.
- **흐름**: EDA→추론 연결 → 표본분포·대수의 법칙·중심극한정리 → 신뢰구간 → 가설검정 → 단순·다중회귀 → 회귀 진단(잔차·공선성) → 설명 vs 예측 → **확인 문제(객관식·서술형)**.
- **관통 서사**: Framingham은 '위험인자(risk factor)' 개념의 발상지 — 오늘의 검정·회귀가 곧 그 위험인자를 발굴하는 절차이고, 그 종착점이 임상 도구 **Framingham Risk Score**입니다.

## 📄 리뷰 논문 · `paper/`

- **To Explain or to Predict?** — Galit Shmueli, *Statistical Science* (2010). [DOI: 10.1214/10-STS330](https://doi.org/10.1214/10-STS330)
- 선정 이유·한 문단 요약: [`paper/논문_선정이유_요약.md`](paper/논문_선정이유_요약.md)
- 요지: **설명(해석)과 예측은 다른 목표** — R²·유의성이 높다고 예측을 잘하는 것은 아닙니다. 과제 §2-E(설명이냐 예측이냐)와 직결됩니다.

## 📝 과제 · `assignment/`

| 파일 | 내용 |
| --- | --- |
| [`assignment.ipynb`](assignment/assignment.ipynb) | 학생 배포용 — 빈칸(`____`, `# TODO`) 채우기 |
| [`solution.ipynb`](assignment/solution.ipynb) | 모범답안 (코드 채워진 판) |
| `data/framingham.csv` | 데이터 (셀 실행 시 공개 URL 자동 로드, 오프라인이면 이 파일로 대체) |

- **유형**: A(기초 체화 — CLT·부트스트랩을 직접 손코딩) + B(도구 활용 — statsmodels·sklearn·scipy).
- **흐름**: 로드 → EDA → 추론(CLT·신뢰구간·t검정) → 회귀(단순·다중·잔차 진단) → 예측(train/test) → **로지스틱 회귀로 진짜 표적 `TenYearCHD` 예측 = Risk Score 엔진**.
- **채점 철학**: 실행은 기본점, **본인 시드(`MY_SEED`)·실행값에 근거한 해석·판단**이 변별점입니다. `MY_SEED`가 사람마다 달라 답이 학생별로 다르며, AI는 검산·설명 도우미로만 씁니다.

### ▶ Colab에서 열기

`assignment.ipynb`를 열고 상단의 **Open in Colab** 배지를 누른 뒤, **맨 위 셀부터 순서대로** 실행하세요. 앞 단계의 결과가 뒤 단계로 이어지는 한 흐름입니다.

---

<sub>ToBig's 26기 정규세션 · 통계적 추론과 회귀분석 · 유주형</sub>
