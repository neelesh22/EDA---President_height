```python
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
sns.set()
```


```python
data= pd.read_csv('president_heights.csv')
```


```python
data.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>order</th>
      <th>name</th>
      <th>height</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>George Washington</td>
      <td>189</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>John Adams</td>
      <td>170</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Thomas Jefferson</td>
      <td>189</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>James Madison</td>
      <td>163</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>James Monroe</td>
      <td>183</td>
    </tr>
  </tbody>
</table>
</div>




```python
height=np.array(data['height'])
```


```python
print('Mean of heights:- ', height.mean() )
print('Standard Deviation of height:- ', height.std())
print('Minimum height:- ', height.min())
print('Maximum height:- ',height.max())
```

    Mean of heights:-  179.73809523809524
    Standard Deviation of height:-  6.931843442745892
    Minimum height:-  163
    Maximum height:-  193



```python
plt.hist(height)
plt.title('Height Distribution of President of USA')
plt.xlabel('height(cm)')
plt.ylabel('Number')
plt.show
```




    <function matplotlib.pyplot.show(close=None, block=None)>




    
![png](output_5_1.png)
    



```python

```
