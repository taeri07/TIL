# Python Object Detection 



![image-20210608141604803](C:\Users\kmh13\AppData\Roaming\Typora\typora-user-images\image-20210608141604803.png)

google.colab & google 드라이브 연결

import os, sys

from google.colab import drive

drive.mount('/content/mnt')

nb_path = '/content/notebook'

os.symlink('/content/mnt/My Drive/Colab Notebooks', nb_path)

sys.path.insert(0, nb_path)



피어슨 상관계수 (Pearson's correlation coefficient)







싸이킷런 데이터 전처리 스케일 조정(스케일러) [sklearn preprocessing StandardScaler MinMaxScaler]

1. pip install sklearn 다운

```
EX 1>

분석시에 변수들이 너무 스케일이 다를 경우

\- 변수들의 단위 차이로 인해 숫자의 스케일이 크게 달라지는 경우



EX 2> 

신경망 학습시에

데이터셋의 값이 들쑥날쑥하거나, 매우 큰 경우에는 cost의 값이 발산하여 정상적인 학습이 이루어지지 않습니다.

0. 데이터셋 만들어주기

from sklearn.datasets import make_blobs
from sklearn.model_selection import train_test_split
X, _ = make_blobs(n_samples= 200, centers= 5, random_state=4, cluster_std=1.5)
plt.scatter(X[:,0],X[:,1])

make_blob 사항 참고

인수:

n_samples : 표본 데이터의 수, 200개

centers : 생성할 클러스터의 수 혹은 중심, [n_centers, n_features] 크기의 배열. 5개

cluster_std: 클러스터의 표준 편차, 1.5

반환값:

X : [n_samples, n_features] 크기의 배열 독립 변수

y : [n_samples] 크기의 배열 종속 변수 (정답레이블 필요시 사용 )

​
```

