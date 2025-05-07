# Eigen for DeepLearning

**以手写数字识别为例，探索Eigen加速矩阵的方法**

关键词:深度学习，手写数字识别，神经网络，卷积层，CMAKE，汇编优化

# From Eigen get how to increase cpp performance
## Eigen 是怎么被加速的
[Eigen加速指导01](https://zhuanlan.zhihu.com/p/426958583)
[Eigen加速指导02](https://www.zhihu.com/question/28571059?sort=created)
[Eigen加速指导03]()

**Eigen加速方法总结:**

1. 调用Intel MKL 线性代数库加速
2. Eigen 原生函数
3. CMKAE 优化:开启-O3加速，编译的时候加上-mavx和-mfma
4. 静态矩阵替代动态矩阵
5. 内存对齐

