<a id="top"></a>

<p align="center">
  <a href="#top" aria-label="Stay on this page">
    <img src="./assets/hero.svg" width="100%" alt="OZ Healthcare Data Lab" />
  </a>
</p>

<h1 align="center">OZ Healthcare Data Lab</h1>

<p align="center">
  <strong>11조 헬스 케어 동아리 · Smoking & Health Data Analysis</strong><br />
  건강검진 데이터에서 흡연 여부와 건강 지표의 관계를 탐색했습니다.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Data-7%2C000%20records-7DD3FC?style=flat-square" alt="7,000 records" />
  <img src="https://img.shields.io/badge/Variables-18-F9A8D4?style=flat-square" alt="18 variables" />
  <img src="https://img.shields.io/badge/Analysis-EDA%20%7C%20Visualization-FBBF24?style=flat-square" alt="EDA and visualization" />
  <img src="https://img.shields.io/badge/Stack-Python%20%7C%20pandas-A7F3D0?style=flat-square" alt="Python and pandas" />
</p>

---

<a id="project"></a>

## Project

최근 건강검진 데이터를 바탕으로 흡연자와 비흡연자의 건강 지표를 비교한 데이터 분석 프로젝트입니다.

분석 대상은 **7,000건, 18개 컬럼**이며 BMI, 혈압, 중성지방, 충치, 공복 혈당, 콜레스테롤 계열 등 건강검진 지표와 흡연 여부가 포함되어 있습니다.

흡연 여부를 단순 예측 대상으로만 보지 않고, **흡연자와 비흡연자 사이에서 어떤 건강 지표의 차이가 관찰되는지**를 시각화하고 정리하는 데 초점을 맞췄습니다.

<p align="center">
  <a href="#project" aria-label="Stay on Project section">
    <img src="./assets/workflow.svg" width="100%" alt="Analysis workflow" />
  </a>
</p>

<a id="findings"></a>

## Findings

<p align="center">
  <a href="#findings" aria-label="Stay on Findings section">
    <img src="./assets/insights.svg" width="100%" alt="Key findings" />
  </a>
</p>

최종 분석 Notebook에서 확인한 대표 결과입니다.

| 항목 | 비흡연 | 흡연 | 관찰 결과 |
|---|---:|---:|---|
| 중성지방 평균 | 113.45 | **150.40** | 흡연자 집단이 높음 |
| 중성지방 중앙값 | 97 | **131** | 흡연자 집단이 높음 |
| 충치 있음 | 19.6% | **28.2%** | 흡연자 집단이 높음 |
| BMI 평균 | 23.81 | **24.73** | 흡연자 집단이 조금 높음 |
| 혈압 평균 | 45.42 | 45.76 | 큰 차이가 보이지 않음 |

BMI 구간별 흡연자 비율은 정상 `30.6%`, 비만전단계 `39.6%`, 1단계 비만 `41.8%`, 2단계 비만 `46.0%`로 높아지는 흐름이 관찰됐습니다. 3단계 비만 구간은 표본이 41명으로 작아 별도로 주의해 해석했습니다.

흡연 여부와의 Pearson 상관계수는 중성지방 `0.25`, BMI `0.13`, 충치 `0.10`, 혈압 `0.02`였습니다. 이 값은 선형적인 동반 변화의 정도이며 인과관계를 의미하지 않습니다.

## Data Preparation

분석 과정에서는 BMI 구간과 연령대를 파생변수로 만들고, 결측값을 변수별로 처리했습니다.

| 변수 | 결측치 | 처리 방법 |
|---|---:|---|
| 혈압 | 140 | 중앙값 |
| 시력 | 140 | 최빈값 |
| 중성지방 | 140 | 연령대별 평균, 이후 전체 평균 |
| 공복 혈당 | 140 | 전체 평균 |

데이터 분포는 비흡연자 4,429명(`63.27%`), 흡연자 2,571명(`36.73%`)으로 균형하지 않았습니다.

## Repository

<p align="center">
  <a href="https://github.com/oz-dongari/smoking_health_data">
    <strong>🚭 smoking_health_data</strong>
  </a>
</p>

| Repository | 내용 |
|---|---|
| [`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data) | 전처리, EDA, 흡연 여부별 비교, 상관관계 분석, 주요 시각화 |

저장소 README에는 최종 Notebook 결과를 기준으로 핵심 수치와 그래프를 정리했습니다. 원본 건강검진 데이터는 공개 저장소에 포함하지 않습니다.

## Limits

이번 분석은 관찰 데이터 기반이므로 인과관계를 판단할 수 없습니다. 발표에서는 혈압 데이터의 성격, 성별 정보 부재, 흡연자·비흡연자 및 연령대의 표본 불균형, 생활 습관 변수 부재를 한계로 정리했습니다.

결과는 특정 건강 행동의 의학적 효과를 확정하는 결론이 아니라 **이 데이터에서 관찰된 관계를 탐색한 결과**로 봅니다.

## Team

| 김진형 | 남한솔 | 안상균 | 이희진 |
|---|---|---|---|
| 11조 헬스 케어 동아리 | 11조 헬스 케어 동아리 | 11조 헬스 케어 동아리 | 11조 헬스 케어 동아리 |

<p align="center">
  <sub>OZ Coding School · AI Healthcare Mini Project</sub>
</p>
