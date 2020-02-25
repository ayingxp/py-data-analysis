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
