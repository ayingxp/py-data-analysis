# matplotlib绘图练习

## 绘图的基本步骤

```python
# 准备数据
x = range(10)
y = range(10)

# 调用plt的相应接口画图
plt.plot(x, y) # plt.bar(x, y), plt.scatter(x, y)

# 添加坐标轴描述信息
plt.ylabel('y label description')
plt.xlable('x label description')

# 添加图片标题

plt.title('my title')

# 坐标轴刻度设置

plt.xticks(x, x_map)
plt.yticks(y, y_map)

# 添加legend
plt.legend()

# 显示图片
plt.show()


```

## 子图调整

```python

from matplotlib.ticker import NullFormatter 


# Format the minor tick labels of the y-axis into empty strings with
# `NullFormatter`, to avoid cumbering the axis with too many labels.

plt.gca().yaxis.set_minor_formatter(NullFormatter())


# Adjust the subplot layout, because the logit one may take more space
# than usual, due to y-tick labels like "1 - 10^{-3}"
plt.subplots_adjust(top=0.92, bottom=0.08, left=0.10, right=0.95, hspace=0.25,
                    wspace=0.35)

```
