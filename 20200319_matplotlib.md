
顏色改成紅色 線條改成虛線-->plot([x], y, [fmt], *, data=None, **kwargs) plt.legend()
```
import matplotlib.pyplot as plt
# 設定資料內容
x  = [1, 2, 3, 4, 5, 6, 7, 8, 9]
y1 = [1, 3, 5, 3, 1, 3, 5, 3, 1]
y2 = [2, 4, 6, 4, 2, 4, 6, 4, 2]
#繪圖
plt.plot(x, y1, label="line L")
plt.plot(x, y2,'r--', label="line H")
plt.plot()

#設定XY軸標籤
plt.xlabel("x axis")
plt.ylabel("y axis")
#設定標題
plt.title("Line Graph Example")
#設定標籤位置
plt.legend(loc='upper left')
#show圖像
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

![BOXPLOT](/page/boxplot.png)
