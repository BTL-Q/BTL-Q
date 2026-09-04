<h1 align="center">BTL-Q</h1>

<p align="center">
  <strong>시장을 데이터로 검증하는 곳</strong><br>
  <sub>전략을 <em>만드는</em> 것보다 <em>의심하고 폐기하는</em> 것에 더 무게를 둡니다.</sub>
</p>

<!-- 한 줄 소개를 넣고 싶으면 이 주석을 지우고 위 문단 아래에 쓰세요.
     예) <p align="center">Computer Vision 엔지니어 · 퀀트 리서치로 이동 중</p>  -->

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas">
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white" alt="SciPy">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" alt="Plotly">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/focus-factor%20%26%20risk%20models-6f42c1?style=flat-square" alt="Factor & Risk Models">
  <img src="https://img.shields.io/badge/focus-backtest%20validation-6f42c1?style=flat-square" alt="Backtest Validation">
</p>

---

## 자산군

방법론이 주인공이고, 자산군은 그것을 검증하는 무대입니다.
같은 코드가 시장을 바꿔 끼워도 돌아가는 것을 목표로 합니다.

| | 지금 | 무엇 때문에 |
|:---|:---:|:---|
| **암호화폐** | ![active](https://img.shields.io/badge/-진행중-2da44e?style=flat-square) | 데이터·주문·호가까지 마찰 없이 열려 있어 **전 과정을 끝까지 돌려보기 좋음**. 24/7이라 표본도 빨리 쌓임 |
| **주식 (KRX · US)** | ![planned](https://img.shields.io/badge/-확장중-0969da?style=flat-square) | 재무·수급처럼 크립토에 **아예 없는 축**이 있음. 상장폐지 이력이 남아 생존편향을 다룰 수 있음 |

> 두 시장은 서로의 약점을 메웁니다.
> 크립토는 마이크로구조 데이터가 열려 있는 대신 역사가 짧고 상폐 코인이 흔적 없이 사라집니다.
> 주식은 그 반대입니다.

---

## 원칙

1. **백테스트는 기본적으로 거짓말을 한다** — 좋은 성적표가 나오면 먼저 버그를 의심합니다.
2. **숫자에는 불확실성을 같이 적는다** — 점추정 옆에 표준오차와 신뢰구간을 둡니다.
3. **파라미터를 고르면 그 순간부터 과최적화다** — In-Sample에서 고른 값이 Out-of-Sample에서 무너지는 정도를 같이 봅니다.
4. **죽은 전략도 기록한다** — 왜 폐기했는지 남기지 않으면 같은 실수를 반복합니다.

---

## 프로젝트

| 저장소 | 무엇인가 | 상태 |
|:---|:---|:---:|
| **[BTC_Dashboard](https://github.com/BTL-Q/BTC_Dashboard)** | 시장모형 회귀로 개별 종목이 기준 자산에 얼마나 끌려다니는지 측정 (β·R²·α·σ_ε) | ![WIP](https://img.shields.io/badge/-작업중-fbca04?style=flat-square) |

<!-- 프로젝트가 늘어나면 여기에 한 줄씩 추가 -->

---

## 로드맵

```
✅  시장모형 회귀 — β · R² · α · σ_ε 분해
🚧  대시보드 공개 배포
⬜  기준 자산 일반화 — BTC / KOSPI / S&P500 교체 가능하게
⬜  롤링 회귀 — 관계가 시간에 따라 얼마나 불안정한지 정량화
⬜  Walk-Forward 검증 프레임
⬜  리스크 사이징 — Kelly · Risk Parity 비교
⬜  주식 트랙 — 재무(DART) · 수급(외인/기관) 팩터
⬜  전략 라이프사이클 파이프라인 (탐색 → 백테스트 → 검증 → 페이퍼)
```

<!-- 연락처를 공개하려면 이 주석을 지우고 아래 형태로 쓰세요.
## 연락
- 이메일 · 블로그 · 링크드인
-->

---

<p align="center">
  <sub>이 저장소들의 코드와 분석은 학습·연구 목적입니다.<br>투자 조언이 아니며, 어떤 수익도 보장하지 않습니다.</sub>
</p>
