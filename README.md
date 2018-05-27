# 6.1
import pandas as pd
import numpy as np
df = pd.DataFrame({'X': [7, 2, 0, 3, 4, 2, 5, 0, 3, 4]})
i = 0
y = 0
arr1 = np.arange(10)

for ele in df['X']:
    y+=1
    if ele != 0:
        arr1[i] = y
    else:
        y = 0
        arr1[i] = y
    i +=1
print(arr1)
