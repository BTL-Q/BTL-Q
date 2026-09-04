<h1 align="center">BTL-Q</h1>

<p align="center">
  <strong>암호화폐 시장을 데이터로 뜯어보는 곳</strong><br>
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
  <img src="https://img.shields.io/badge/market-Upbit%20KRW-1f6feb?style=flat-square" alt="Upbit KRW">
  <img src="https://img.shields.io/badge/focus-factor%20%26%20risk%20models-6f42c1?style=flat-square" alt="Factor & Risk Models">
  <img src="https://img.shields.io/badge/hours-24%2F7-2da44e?style=flat-square" alt="24/7">
</p>

---

## 원칙

<table>
<tr>
<td width="50%" valign="top">

### 1. 백테스트는 기본적으로 거짓말을 한다

Look-ahead bias, 생존 편향, 과최적화.
좋은 성적표가 나오면 **먼저 버그를 의심**합니다.
포지션은 항상 `signal.shift(1)`,
수수료와 슬리피지는 처음부터 포함합니다.

</td>
<td width="50%" valign="top">

### 2. 숫자에는 불확실성을 같이 적는다

β 하나만 쓰지 않고 **표준오차와 신뢰구간**을 함께 둡니다.
p값이 유의하지 않으면 화면에 "무의미"라고 적습니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 3. 파라미터를 고르면 그 순간부터 과최적화다

In-Sample에서 고른 조합이
Out-of-Sample에서 **얼마나 무너지는지**를 같이 보여줍니다.

</td>
<td width="50%" valign="top">

### 4. 죽은 전략도 기록한다

왜 폐기했는지 남기지 않으면
**같은 실수를 반복**합니다.

</td>
</tr>
</table>

---

## 프로젝트

| 저장소 | 무엇인가 | 상태 |
|:---|:---|:---:|
| **[BTC_Dashboard](https://github.com/BTL-Q/BTC_Dashboard)** | 코인 간 영향력 분석 — 시장모형 회귀(β·R²)로 *"이 코인이 기준 코인에 얼마나 끌려다니는가"* 를 측정 | ![WIP](https://img.shields.io/badge/-작업중-fbca04?style=flat-square) |

<!-- 프로젝트가 늘어나면 여기에 한 줄씩 추가 -->

---

## 지금 파고 있는 것

### 시장모형 회귀 — 알트코인은 정말 독립적인 베팅인가

$$r_{coin,t} = \alpha + \beta \cdot r_{base,t} + \varepsilon_t$$

기준 코인(BTC 등) 수익률에 다른 코인을 회귀시켜 세 가지를 분리합니다.

| 기호 | 의미 | 읽는 법 |
|:---:|:---|:---|
| **β** | 민감도 | 기준 코인이 1% 움직일 때의 반응 폭 |
| **R²** | 영향력 | 이 코인 움직임 중 기준 코인으로 설명되는 비율 |
| **σ_ε** | 고유 변동성 | 기준 코인을 제거하고 남은 몫 — 분산투자로 줄일 수 있는 부분 |

> **β와 R²는 서로 독립입니다.**
> 크게 반응하는 것(β)과 충실하게 따라가는 것(R²)은 다른 질문이고,
> 포트폴리오를 짤 때 실제로 중요한 건 후자입니다.

**여기서 나온 것** — 관측 주기를 짧게 자를수록 측정되는 상관이 깎여 나갑니다 (Epps effect).
같은 코인이 일봉에서 R² 58%인데 시간봉에서는 50%로 떨어집니다.
*"이 코인의 베타는 얼마"* 라는 문장은 **어느 주기, 어느 구간에서** 를 빼면 의미가 없습니다.

---

## 로드맵

```
✅  코인 영향력 분석 — 시장모형 회귀 (β · R² · α · σ_ε)
🚧  대시보드 공개 배포
⬜  롤링 회귀 — 관계가 시간에 따라 얼마나 불안정한지 정량화
⬜  Walk-Forward 검증 프레임
⬜  리스크 사이징 — Kelly · Risk Parity 비교
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
