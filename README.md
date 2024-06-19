# 금융 사막화에 따른 ​방문형 은행 장소 추천 (전라남도 대상)

## 금융 사막화란?
- 은행이나 증권사 등 금융기관의 유인 점포가 수도권에만 남고 농촌 등 비수도권에선 사라지는 현상​
- 금융소외계층의 금융 접근성은 더욱 악화되며 서비스 선택 권리도 제한​

## 문제 분석 및 목표 방향
![image](https://github.com/YuHan-J-Nam/Jeonnam_Banking_Desert_Analysis/assets/43714833/6522e7b3-f35c-417f-9a5f-7a2c85e62bd7)

![image](https://github.com/YuHan-J-Nam/Jeonnam_Banking_Desert_Analysis/assets/43714833/d20fa820-e10e-4540-975d-e0d180f5f894)

## 분석 파일 목록 및 설명
### 1. housing_data_preprocessing.ipynb
전라남도의 법정동 기준 인구 데이터를 전처리

### 2. geo_data_preprocessing.ipynb
전라남도의 개별/공동주택 정보와 은행 위치 정보를 결합하여 다음 정보를 추출:
- 특정 주소를 기준으로 반경 x km 내의 은행 개수 파악
- 특정 주소를 기준으로 가장 가까운 은행까지의 거리 및 대중교통 소요시간 계산

### 3. k_means_cluster_analysis.ipynb
전처리한 데이터를 기반으로 전라남도 내의 금융 사막화 지역을 군집화를 통해 파악

### 4. economic_data_preprocessing.ipynb
각 행정구역 별 산업 경제지표 데이터를 전처리

### 5. DBSCAN_cluster_analysis.ipynb
금융 사막화 지역으로 판별된 곳들을 지리적 위치를 기준으로 군집화하고 경제지표를 반영
