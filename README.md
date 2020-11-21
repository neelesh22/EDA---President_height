# EDA---President_height
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
sns.set()

data= pd.read_csv('president_heights.csv')

data.head()

	order 	name 	height
0 	1 	George Washington 	189
1 	2 	John Adams 	170
2 	3 	Thomas Jefferson 	189
3 	4 	James Madison 	163
4 	5 	James Monroe 	183

height=np.array(data['height'])

print('Mean of heights:- ', height.mean() )
print('Standard Deviation of height:- ', height.std())
print('Minimum height:- ', height.min())
print('Maximum height:- ',height.max())

Mean of heights:-  179.73809523809524
Standard Deviation of height:-  6.931843442745892
Minimum height:-  163
Maximum height:-  193

plt.hist(height)
plt.title('Height Distribution of President of USA')
plt.xlabel('height(cm)')
plt.ylabel('Number')
plt.show

