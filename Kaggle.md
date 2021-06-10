20210607



PRACTICE 

1. 이번주 가장 많은 손님이 예상되는 요일은?

   -토요일

2. 가장 많은 손님이 예상되는 요일에 no(#) 예상되는 팀수?

   -87

3. 가장 많은 손님이 예상되는 요일의 예상 매출은?

   1740

4. 가장 많은 손님이 예상되는 요일의 예상 되는 tip $?

   261





## KAGGLE

https://www.kaggle.com/taeri07/creating-reading-and-writing/edit



1. PANDA pkg 불러오기

   ```python
   import panda as pd
   ```











import pandas as pd
pd.set_option('max_rows', 5)
from learntools.core import binder; binder.bind(globals())
from learntools.pandas.creating_reading_and_writing import *
print("Setup complete.")







ingredients = pd.Series(['4 cups', '1 cup', '2 large', '1 can'
],index=['Flour','Milk','Eggs','Spam'], name='Dinner')
q3.check()
ingredients