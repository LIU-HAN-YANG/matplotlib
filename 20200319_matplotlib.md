
顏色改成紅色 線條改成虛線-->plot([x], y, [fmt], *, data=None, **kwargs) plt.legend()
```
import matplotlib.pyplot as plt
 
x  = [1, 2, 3, 4, 5, 6, 7, 8, 9]
y1 = [1, 3, 5, 3, 1, 3, 5, 3, 1]
y2 = [2, 4, 6, 4, 2, 4, 6, 4, 2]
plt.plot(x, y1, label="line L")
plt.plot(x, y2,'r--', label="line H")
plt.plot()

plt.xlabel("x axis")
plt.ylabel("y axis")
plt.title("Line Graph Example")
plt.legend(loc='upper left')
plt.show()
```

boxplot箱形圖 (Box plot):使用matplotlib.pyplot.boxplot

```
import numpy as np
import matplotlib.pyplot as plt

# Fixing random state for reproducibility
np.random.seed(19680801)
people=[178 , 164 , 159 , 162 , 182 , 
             179 ,  166 , 168 , 173 , 165]

fig1, ax1 = plt.subplots()

plt.ylabel("hight")
ax1.set_title('people_hight')
ax1.boxplot(people)


```

![BOXPLOT](/matplotlib/page/boxplot.png)
