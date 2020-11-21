

import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
sns.set()

data= pd.read_csv('president_heights.csv')

data.head()

height=np.array(data['height'])

print('Mean of heights:- ', height.mean() )
print('Standard Deviation of height:- ', height.std())
print('Minimum height:- ', height.min())
print('Maximum height:- ',height.max())

plt.hist(height)
plt.title('Height Distribution of President of USA')
plt.xlabel('height(cm)')
plt.ylabel('Number')
plt.show

 

