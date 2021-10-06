# 과제 4: 미국 대통령들의 키는 얼마나 컸을까?

역대 미국 대통령들의 신장(height) 데이터 ```president_height.csv``` 가 있습니다.

해당 데이터를 이용하여 역대 대통령들의 키와 관련된 기술통계(descriptive statistics) 분석을 수행하고 그 결과를 시각화하세요.

## 준비사항
### 1. 필수 라이브러리 설치

과제 수행에 필요한 라이브러리(```numpy, pandas, matplotlib, seaborn```)들을 모두 설치하세요(이미 설치되어 있는 상태면 skip).

- 설치방법 1: jupyter lab 브라우저의 독립된 셀에서 명령어 실행(셀 안에 명령어 외의 다른 코드 포함 X)
- 설치방법 2: Anaconda->Environments->Open Terminal 실행 후 터미널에서 명령어 실행

#### 예: pandas 설치 명령어
```pip install pandas```

### 2. 신장 데이터 저장

2.1 신장 데이터 파일 링크: [president_height.csv](https://github.com/gurami85/lectures/blob/main/data/president_heights.csv)

2.2 해당 페이지에서 'Raw' 메뉴 클릭하여 파일 텍스트 내용을 확인

2.3 우클릭->다른이름으로 저장->```president_heights.csv``` 파일이름으로 저장

2.4 Jupyter Lab 에서 ```data``` 폴더 생성

2.5 ```president_heights.csv``` 를 생성한 ```data``` 폴더에 복사

## 기술통계

### 3. 데이터 로딩

3.1 ```numpy``` 와 ```pandas``` 를 임포트

```python3
import pandas as pd
import numpy as np
```

3.2  ```pandas``` 라이브러리를 이용하여 신장 데이터(```president_heights.csv```)를 불러오기

```python3
data = pd.read_csv('data/president_heights.csv')
```

3.3 데이터 불러오기가 정상적으로 완료되었다면  ```data.head()``` 코드를 실행하여 데이터의 일부를 출력

#### 예상 출력결과

|order|name|height(cm)|
|---|---|---|
|1|George Washington|189|
|2|John Adams|170|
|3|Thomas Jefferson|189|
|4|James Madison|163|
|5|James Monroe|183|


