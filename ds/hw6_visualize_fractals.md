## <strong> 과제 6: 프랙털 시각화 </strong>
---
<strong>프랙털</strong>(fractal)은 수학, 기하학 연구 분야 중 하나로서, <strong>자기유사성</strong>을 갖는 기하학적 구조를 말합니다. 쉽게 말하면 어떤 도형의 작은 일부를 확대해 봤을 때 그 도형의 전체 모습이 똑같이 반복되는 특징을 가집니다. 프랙털 구조는 간단한 수학적 규칙이 반복 적용됨으로써 생성되며, 나무의 구조와 해안선의 모양과 같이 자연에서도 다양한 프랙털 패턴들이 발견됩니다.

본 예제 코드에서 NumPy 유니버설 함수 관련 코드를 완성하여  간단한 프랙털 구조를 시각화하세요.
+ 출처: NumPy 공식 웹사이트
+ 유의사항: 본 과제는 프랙털 이론과 시각화 방법을 배우는 것이 목적이 아니므로, NumPy 유니버설 함수를 사용하는 부분을 제외한 나머지 코드는 완성된 형태로 제공됩니다👽.  

<strong> 필요한 라이브러리 </strong>
+ ```numpy```: 다차원 배열 연산
+ ```matplolib```: 시각화
+ ```mpl_toolkits.axes_grid1```: ```matplotlib``` figure의 축 레이블 옵션

```python
import numpy as np  
import matplotlib.pyplot as plt  
from mpl_toolkits.axes_grid1 import make_axes_locatable
```

<strong> 시각화 설정 코드 </strong> : 별도의 윈도우 창에서 시각화 결과를 출력하는 코드이며, 시각화 결과가 제대로 출력되지 않는 경우에는 ```%matplotlib qt5``` 코드를 삭제하고 커널을 재시작(Kernel-Restart Kernel)하기 바랍니다.

```python
%matplotlib qt5
%config InlineBackend.figure_format = 'svg'

plt.rcParams['figure.figsize'] = [12, 5]
plt.rcParams['font.size'] = 13
plt.ion()
```
