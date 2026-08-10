<p align="center">
  <a href="#_" aria-label="OZ Healthcare Data Lab visual"><img src="./assets/hero.svg" width="100%" alt="OZ Healthcare Data Lab" /></a>
</p>

<p align="center">
  <strong>OZ Coding School · AI Healthcare Mini Project · Team 11</strong><br />
  건강검진 데이터에서 흡연 여부와 건강 지표의 관계를 탐색하고 시각화했습니다.
</p>

---

## 프로젝트

[`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data)는 **7,000건, 18개 컬럼**의 건강검진 데이터를 바탕으로 흡연자와 비흡연자의 건강 지표 차이를 살펴본 프로젝트입니다. BMI, 중성지방, 충치, 혈압을 중심으로 전처리, EDA, 집단 비교와 상관관계 분석을 진행했습니다.

예측 모델의 성능을 겨루기보다, **이 데이터에서 어떤 차이가 실제로 관찰되는지 이해하고 설명하는 것**에 초점을 맞췄습니다.

<p align="center">
  <a href="#_" aria-label="Analysis workflow visual"><img src="./assets/workflow.svg" width="100%" alt="Analysis workflow" /></a>
</p>

## 핵심 결과

<p align="center">
  <a href="#_" aria-label="Key findings visual"><img src="./assets/insights.svg" width="100%" alt="Key findings" /></a>
</p>

| 항목 | 비흡연 | 흡연 |
|---|---:|---:|
| 중성지방 평균 | 113.45 | **150.40** |
| 충치 있음 | 19.6% | **28.2%** |
| BMI 평균 | 23.81 | **24.73** |
| 혈압 평균 | 45.42 | 45.76 |

BMI 구간별 흡연자 비율은 정상 `30.6%` → 비만전단계 `39.6%` → 1단계 비만 `41.8%` → 2단계 비만 `46.0%`로 높아지는 흐름이 관찰됐습니다. 3단계 비만은 표본이 41명으로 작아 추세 해석에 주의했습니다.

흡연 여부와의 Pearson 상관계수는 중성지방 `0.25`, BMI `0.13`, 충치 `0.10`, 혈압 `0.02`였습니다. 세부 전처리와 시각화 결과는 프로젝트 저장소 README에서 확인할 수 있습니다.

## 해석 범위

이번 분석은 관찰 데이터 기반이므로 집단 간 차이와 상관관계는 확인할 수 있지만 인과관계를 단정할 수는 없습니다. 발표에서는 혈압 데이터의 성격, 성별 정보 부재, 흡연 여부와 연령대의 표본 불균형, 생활 습관 변수 부재를 주요 한계로 정리했습니다.

## Repository

### [`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data)

전처리, EDA, 흡연 여부별 비교, 상관관계 분석과 주요 시각화를 정리한 공개 저장소입니다. 원본 건강검진 데이터는 포함하지 않습니다.

## Team

**김진형 · 남한솔 · 안상균 · 이희진**  
OZ Coding School · 11조 헬스 케어 동아리

<p align="center">
  <sub>Smoking & Health Data Analysis · AI Healthcare Mini Project</sub>
</p>