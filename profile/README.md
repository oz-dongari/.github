<p align="center">
  <a href="#_" aria-label="OZ Healthcare Data Lab visual"><img src="./assets/hero.svg" width="100%" alt="OZ Healthcare Data Lab" /></a>
</p>

<p align="center">
  <strong>OZ Coding School · AI Healthcare Mini Project · Team 11</strong><br />
  건강검진 데이터 기반 흡연 여부별 건강 지표 분석·시각화
</p>

---

## 프로젝트

[`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data)  
**7,000건 · 18개 컬럼**  
BMI · 중성지방 · 충치 · 혈압 중심 전처리 · EDA · 집단 비교 · 상관관계 분석

**분석 초점:** 예측 성능 경쟁보다 관찰 패턴의 구조화·해석

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

**BMI 구간별 흡연자 비율**  
정상 `30.6%` → 비만전단계 `39.6%` → 1단계 비만 `41.8%` → 2단계 비만 `46.0%`  
3단계 비만 `43.9%` (`n=41`) — 소표본으로 추세 해석 제외

**Pearson r**  
중성지방 `0.25` · BMI `0.13` · 충치 `0.10` · 혈압 `0.02`

세부 전처리·시각화: [`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data)

## 해석 범위

관찰 데이터의 집단 차이·상관관계. 인과 추론 제외.

**주요 한계:** 혈압 변수 성격 · 성별 정보 부재 · 흡연 여부/연령대 표본 불균형 · 생활 습관 변수 부재

## Repository

### [`smoking_health_data`](https://github.com/oz-dongari/smoking_health_data)

전처리 · EDA · 흡연 여부별 비교 · 상관관계 · 주요 시각화  
원본 건강검진 데이터 미포함

## Team

**김진형 · 남한솔 · 안상균 · 이희진**  
OZ Coding School · 11조 헬스 케어 동아리

<p align="center">
  <sub>Smoking & Health Data Analysis · AI Healthcare Mini Project</sub>
</p>