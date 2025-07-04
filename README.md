
# 배당주 투자 시뮬레이터 (Dividend Stock Investment Simulator)

### 성장주에 투자해 자산을 크게 불릴 것인가(애플, MSFT) vs 고배당주에 투자해 안정적인 현금 흐름을 만들 것인가(QYLD, JEPI)
이 프로젝트는 다양한 배당주에 대한 미래 주가와 투자 성과를 시뮬레이션하고 분석하기 위해 제작되었습니다. 기하 브라운 운동(Geometric Brownian Motion) 모델을 사용하여 특정 기간 후의 주가를 예측하고, 이를 바탕으로 총자산, 누적 배당금, 투자 위험 등 다양한 지표를 계산하고 시각화합니다.

## 🚀 주요 기능

-   **미래 주가 시뮬레이션**: GBM 모델을 기반으로 N년 후의 주가를 확률적으로 시뮬레이션합니다.
-   **통계 분석**: 시뮬레이션 결과를 바탕으로 표본평균, 분산, 표준편차 등 주요 통계 지표를 계산합니다.
-   **자산 성장 예측**: 초기 투자금에 대한 미래 평가액, 누적 배당금, 총자산을 예측하여 보여줍니다.
-   **배당 목표 분석**: 월별 목표 배당금을 달성하기 위해 필요한 초기 투자금을 계산합니다.
-   **위험 및 가치 평가**: 주가 상승률, 변동성, PER(주가수익비율) 등을 통해 투자의 기대수익과 위험도를 분석합니다.
-   **데이터 시각화**: 분석 결과를 막대그래프와 히스토그램으로 시각화하여 직관적인 이해를 돕습니다.

## 🛠️ 사용 기술

-   **Python**: 데이터 분석 및 시뮬레이션
-   **Pandas & NumPy**: 데이터 처리 및 수치 연산
-   **Matplotlib**: 데이터 시각화
-   **yfinance**: 최신 주가 및 기업 정보 수집

## ⚙️ 실행 방법

1.  Jupyter Notebook 환경에서 `이예림_202322091_금프1_기말프로젝트(복제).ipynb` 파일을 엽니다.
2.  아래 라이브러리들이 설치되어 있는지 확인합니다. 없다면 설치가 필요합니다.
    ```bash
    pip install numpy pandas matplotlib yfinance
    ```
3.  노트북 상단의 설정 부분에서 원하는 주식 `TICKERS`와 파라미터를 수정할 수 있습니다.
4.  Jupyter Notebook의 모든 셀을 순서대로 실행하면 분석 결과와 그래프를 확인할 수 있습니다.

## 📊 분석 결과 예시

이 시뮬레이터를 실행하면 다음과 같은 5가지 핵심 분석 결과를 얻을 수 있습니다.

1.  **10년 후 총자산 비교**: 동일 금액 투자 시, 각 종목의 10년 후 총자산을 비교하여 최고의 성장주를 찾습니다.
2.  **총자산 상세 요약**: 총자산이 주가 상승과 배당금 중 어디에서 비롯되었는지 상세 수치를 보여줍니다.
3.  **목표 배당금 필요 투자금**: 월 목표 배당금을 받기 위해 종목별로 얼마를 투자해야 하는지 계산합니다.
4.  **주가 분포 통계 요약**: 미래 주가의 평균, 변동성, 상승률, PER 등을 통해 성장 잠재력과 위험을 수치로 확인합니다.
5.  **주가 분포 히스토그램**: 미래 주가 분포를 시각화하여 변동성의 크기를 직관적으로 파악합니다.

![image](https://github.com/user-attachments/assets/59f7c946-50c0-446f-9698-5cf9f91aff2a)


