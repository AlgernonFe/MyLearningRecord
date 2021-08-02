\documentclass[UTF8, a4paper, 10pt]{article}
\usepackage{ctex}
\usepackage{fancyhdr}
\usepackage{multicol}
\usepackage{lastpage}
\usepackage[subfigure, AllowH]{graphfig}
\usepackage{geometry}
\geometry{left = 3.18cm, right = 3.18cm, top = 2.54cm, bottom = 2.54cm}
\usepackage{graphicx}
\usepackage{CJK}
\renewcommand{\baselinestretch}{1.5}
\parindent 22pt
\begin{document}
\begin{center}
\LARGE\textbf{Machine Learning学习记录}
\end{center}
\tableofcontents
\clearpage
\section{2021.8.1}吴恩达机器学习系列课程1-1至4.8节

\subsection{监督学习与无监督学习}
\subsubsection{监督学习}
\begin{itemize}
    \item 回归问题(Regression problem)
    \item 分类问题(Classification problem)
\end{itemize}

\subsubsection{无监督学习}
\begin{itemize}
    \item 聚类算法
    \item 鸡尾酒会问题
\end{itemize}

\subsection{线性回归算法(Batch)}
\begin{enumerate}
    \item 假设函数: $h_{\theta}(x)$
    \item 代价函数：$J(\theta) = \frac{1}{2m}\sum^n_{i=1}(h_{\theta}(x^{(i)}-y^{(i)}) ^2$
    \item 梯度下降：$\theta_j := \theta_j - \alpha\frac{\partial J(\theta_0, \theta_1,\cdots, \theta_n)}{\partial \theta_j}$
    \\其中$\alpha$为学习率，控制更新$\theta_j$的幅度。
\end{enumerate}
\subsection{特征缩放}
\subsection{正规方程解析解}矩阵方法，
求出最优$\vec{\theta}$:
$$\vec{\theta} = (X^T X)^{-1}X^T\vec{y}$$
\subsection{Octave下载与基本语法学习}

\section{2021.8.23}
安装Octave环境；下载编程作业；吴恩达机器学习系列课程5.1-5.3
\subsection{Octave语法学习}
使用Octave进行矩阵/向量的生成与运算操作。
\end{document}

