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
吴恩达机器学习系列课程5.4-5.6，编程作业1提交
## Matlab绘图、控制语句、函数学习

# 2021.8.4
吴恩达机器学习系列课程6.1-6.7，随堂测试提交
## Logistic Regression
- 0 < $h_\theta(x) < 1$
- $h_\theta = \frac{1}{1+e^{\theta^Tx}}$
- $P(y = 0| x; \theta) + P(y = 1| x; \theta) = 1$
## 决策边界
## 代价函数
- Training Set： ${(x^{(1)}, y^{(1)}), (x^{(2)}, y^{(2)})\cdots  (x^{(m)}, y^{(m)})}$
- $h_\theta(x) = \frac{1}{1 + e^{-\theta^Tx}}$
- Cost function: $J(\theta) = \frac{1}{m}\sum^m_{i = 1}\frac{1}{2}(h_\theta(x^{(i)} - y^{(i)})^2$,——非凸函数，梯度下降不保证得到全局最优
- 变换为凸函数: 
  <br>$Cost(h_\theta(x), y) = -log(h_\theta(x)), y = 1$
  <br>$Cost(h_\theta(x), y) = -log(1 - h_\theta(x)), y = 0$
- 代价函数优化：$Cost(h_\theta(x), y) = ylog(h_\theta(x)) - (1-y)log(1 - h_\theta(x))$
## 最小化代价函数：梯度下降
Repeat{$\theta_j := \theta_j - \alpha\frac{\partial J(\theta_0, \theta_1,\cdots, \theta_n)}{\partial \theta_j}$}
## 高级优化：提高回归速度
Conjugate descent, BFGS, L-BFGS
<br>优点：无需手动选择学习率，算法自动尝试 $\alpha$并选择
## 多元分类：一对多
将某一样本设置为正类别，其余看做负类别，进行多次二元分类

# 2021.8.5
吴恩达机器学习系列课程7.1-8.4，编程作业2
## 过拟合Overfitting
## 正则化
为参数加上惩罚项，使可能导致过拟合的参数尽量小
## 线性回归的正则化
- 梯度下降
<br> $\theta_j = \theta(1-\alpha\frac{\lambda}{m}) - \frac{\alpha}{m}\sum^m_{i = 1}(h_\theta(x^{(i)} - y^{(i)})x_j^{(i)}$
- 解析方法
## 逻辑回归的正则化

## 神经网络
前向传播