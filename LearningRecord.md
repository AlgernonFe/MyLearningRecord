# 2021.8.1
吴恩达机器学习系列课程1-1至4.8节

##  监督学习与无监督学习
1. 监督学习
   - 回归问题(Regression problem)
   - 分类问题(Classification problem)
2. 无监督学习
   - 聚类算法
   - 鸡尾酒会问题

## 线性回归算法(Batch)
1. 假设函数: $h_{\theta}(x)$
2. 代价函数：$J(\theta) = \frac{1}{2m}\sum^n_{i=1}(h_{\theta}(x^{(i)}-y^{(i)}) ^2$
3. 梯度下降：$\theta_j := \theta_j - \alpha\frac{\partial J(\theta_0, \theta_1,\cdots, \theta_n)}{\partial \theta_j}$
<br>其中$\alpha$为学习率，控制更新$\theta_j$的幅度。
4. 特征缩放
5. 正规方程解析解：矩阵方法
<br> 求出最优$\vec{\theta}$: $\vec{\theta} = (X^T X)^{-1}X^T\vec{y}$

# 2021.8.2
安装Octave环境；下载编程作业；吴恩达机器学习系列课程5.1-5.3
## Octave语法学习
使用Octave进行矩阵/向量的生成与运算操作。

# 2021.8.3
吴恩达系列课程5.1-5.3，编程作业1提交
## matlab绘图、函数功能学习与运用