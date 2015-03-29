---
layout: page
title: data
permalink: /data/
---  

### Unit 1

#### 1 - 1 - Unit 1- Introduction (3-28)

![主要内容](http://ww3.sinaimg.cn/mw1024/889c2cc9gw1eq14eccnd2j20dw07t759.jpg)

---

#### 1 - 2 - Unit 1, Part 1- (1) Data Basics (5-21)

* **Data Matrix**：数据存在的一种形式，一行为一条观察数据，一列为一个变量（像Excel表格那样）
* **Variable**：分为**numerical（数量型变量）**和**categorical（类别变量）**。
  * numerical又分为continuous（连续的）和discrete（离散的）；
  * categorical又分为ordinal（有序的）和regular categorical（无序的）
* 以2011年Google transparency report为例，介绍一些数据方面的基本概念
* 变量之间相互联系：**associated**/**dependent**.association进一步可以被描述为positive/negative
![photo](http://ww3.sinaimg.cn/mw1024/889c2cc9gw1eq14egy5gpj20dw07twf9.jpg)

---

#### 1 - 3 - Unit 1, Part 1- (2) Observational Studies & Experiments (4-39)研究方法

* **observational（观察性研究）**：直接取现实中的数据，不在研究过程中控制变量的实现，这种研究`只能探究相关性而对因果性无力`（如下图），observational又分为:
  * **retrospective（回顾）**－依赖以前的数据以及
  * **prospective（预期）**－在研究中收集新的数据。
* **experiment**：在实验过程中控制实现变量的过程
* 区别是变量是否受researcher控制。因为observational的结果有可能是由于其他未受控制的变量导致，而experiment的各变量相对得到控制，得出的结论也相对具有因果性。
![混淆变量](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eq14xhx1caj20dw07tmxt.jpg)
![混淆变量](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eq14xjbi8uj20dw07taat.jpg)
![无因果性](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eq14eeg9fej20dw07t3zc.jpg)

---

#### 1 - 4 - Unit 1, Part 1- (3) Sampling and Sources of Bias (7-33) 取样和样本偏性

* 将人口普查中的取样类比于烹饪时尝一小口而无需吃掉整锅来说明取样
* **Sampling Bias 样本偏性**：可能来源于取样的convenience sample(便利性)、non-response(无响应)、voluntary response(自愿响应)等；例子：CNN调查是否入侵叙利亚调查（只有上CNN网站的人参与调查）、1936总统选举调查(杂志做的调查与实际结果相差很多，最终FDR富兰克林罗斯福获选，杂志倒闭)
* 取样方法：
  * **simple random sample (SRS)**：不做控制随机地取样；
  * **stratified sample 分层**：按相似性分成若干的阶层(homogenous strata)，在各阶层内取样；
  * **cluster sample 聚类**：随机分成若干堆，随机取一些堆，再在这些堆内取样.与stratified不同的是，cluster每堆内不是homogenous，但是各堆之间都相似。通常用cluster的取样方法是出于经济原因，比如每个城市分不同的几个相似区域做调查就好。
  
---



#### 1 - 5 - Unit 1, Part 1- (4) Experimental Design (2-59) 实验设计

* 设计原则：**control**：比较实验组与对照组；**randomize**：保证数据的随机性；**replicate**：足够大的实验量；**block**：消除无关变量的影响
* 专业运动员与业务运动员使用能量gel的例子。其中blocking variables是专业（业余），而是否使用能量gel则是explantory variables (factors),如下图：
![blocking vs. explanatory variables](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eq1qjqd5icj20dw07tjs8.jpg)
* **安慰剂效应**：多用于药物实验，给对照组无关的；blinding；double-blind
* **盲或双盲**以及**安慰剂**：在需要从人的主观感受中剥离客观结论的社会性研究（比如药物实验）中，如果被试的主观感受会影响数据结果，就需要给予对照组无实质作用的安慰剂，并且对被试隐藏其属于实验组还是对照组的信息，以区分实验组的变化和安慰剂效应，这就叫blind experiment；更进一步，如果研究者的主观感受也会影响实验结果，则对研究者也隐藏实验与对照的分组信息，这就是通常说的双盲实验.

---



#### 1 - 6 - Unit 1, Part 1- (Spotlight) Random Sample Assignment (3-33)

**random sample** and **random assignment**的区别，前者是取样方法中的一种，即从总体中取样本，每个样本被抽取的概率是一样的，用以generalization；后者是experiment中的必备步骤，也就是将样本随机分为treatment和control两组，用以causality（因果性）。
![random sample vs. random assignment](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eq1qjrr22dj20dw07tmxu.jpg)

---



#### 1 - 7 - Unit 1, Part 2- (1) Visualizing Numerical Data (10-27) 数量型数据的可视化

* **Scatter Chart散点图**：可以从中归纳两个变量的相关性。相关性有几个性质：正相关/负相关、形状（线性、非线性）、强相关/弱相关，并且要排除异常值
* **Histogram直方图**：可以给出一个数据密度的视图，并且可以观察：
* Skewness偏度：描述了数据密度的左右分布，left skewed左偏/right skewed右偏/symmetric对称
* Modality形态：正态分布/均匀分布/双峰分布/多峰分布等等.区间划分不能过宽或过窄.
![Modality](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eq3cxhmsh7j20dw07tq3o.jpg)
* **Dot Plot**：用于处理几个分离的变量值，不太适用于样本量太大时
* **Box Plot箱形图**：highlighting ourlier.箱子的左中右三条线用来显示包括中位数在内的四分位数，箱子的宽度是四分差（IQR）。可以由它近似地画出分布曲线的形态.
![BP](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eq3cxkcz4sj20dw07tdgr.jpg)
![BP](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eq3cxik7tij20dw07tgm3.jpg)  
* **Intensity Map** 
![IM](http://ww3.sinaimg.cn/mw1024/889c2cc9gw1eq3cxlg091j20dw07tdgq.jpg) 
   
> 脑洞：散点图适用于三维数据集，但其中只有两维需要比较。比如下图是各国的医疗支出与预期寿命，三个维度分别为国家、医疗支出、预期寿命，只有后两个维度需要比较。为了识别第三维，可以为每个点加上文字标示，或者不同颜色。
![散点图](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eq2z6hpazfj20dw07tgmb.jpg)

> 气泡图是散点图的一种变体，通过每个点的面积大小，反映第三维。卡特里娜飓风的路径，三个维度分别为经度、纬度、强度。点的面积越大，就代表强度越大。因为用户不善于判断面积大小，所以气泡图只适用不要求精确辨识第三维的场合。如果为气泡加上不同颜色（或文字标签），气泡图就可用来表达四维数据。比如下图就是通过颜色，表示每个点的风力等级。    
![气泡图](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eq2z6jhketj20dw09o75e.jpg)
![气泡图](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eq2z6l1tjoj20dw08fgmh.jpg)
![气泡图](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eq2z6ol65qj20dw0el768.jpg)


---



#### 1 - 8 - Unit 1, Part 2- (2) Measures of Center (4-20) “中心”的测量

* Skewness、Modality对于确定“中心”是有用的
* 测量“中心”的几种方式：**mean均值**、**median中位数(50th percentile)**、**mode众数**
* Measures of Center：如果对“中心”的测量是从样本数据算出的，就叫它为**sample statistic样本统计量**，样本统计量是我们想知道的**population parameter总体统计量**的一个**point estimate点估计**，point estimate可以看作基于样本的有限数据对整体的性质做出了一个good guess。在符号上，通常以拉丁字母表示sample statistic，以希腊字母表示population parameter。比如 **$$\overline{x}$$** 表示sample mean, $$\mu$$ 表示population mean
* skewness与mean/median大小的关系如下：左偏，mean在median左边（小于）；右偏mean在median右边（大于）。

![skewness](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eq3cxm1nvsj20dw07t0te.jpg)

---



#### 1 - 9 - Unit 1, Part 2- (3) Measures of Spread (6-56) 离散度测量

离散度测量4种：总之越多的观察值离center近，离散度越小。

1. range (max - min) 
2. **variance方差**：roughly the average squared deviation from the mean，因为经过了乘方，消除了正负偏离的影响，而且偏离大的数据得到了更大的体现。$$s^{2}$$ 表示sample variance，$$\sigma ^{2}$$ 表示population variance 

$$ s ^{2} = \frac{\sum_{1}^{n=1} (x_i - \overline{x})^{2}}{n-1} $$  

3. **standard deviation标准差**：方差的正平方根
4. **inter-quartile range (IQR)四分位数间距**: IQR = Q3 - Q1. IQR比第1点range算离散度更可靠，是因为IQR不依赖endpoint，不受outlier影响。
**variability** vs. **diversity多样性**：这里举了彩色汽车的例子，针对英里数变量比较了Variability，针对颜色变量比较了Diversity
![cars](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eqc1finhz8j20dw07twfb.jpg)


---



#### 1 - 10 - Unit 1, Part 2- (4) Robust Statistics (1-25) 稳健统计量

* 若对样本中的某一个数据做扰动修改，以上提出的统计量是否足够稳健、抗干扰呢？
* 稳健统计量：中位数、四分差
* 不稳健统计量：平均值、标准差
![cars](http://ww3.sinaimg.cn/mw1024/889c2cc9gw1eqc9sr272jj20dw07t74x.jpg)

---



#### 1 - 11 - Unit 1, Part 2- (5) Transforming Data (3-05) 数据转换

针对降低偏度强烈等情况的数据，做一个函数转换，以降低对建模造成的难度

* log对数转换：最常用的一种转换，适用于数据为正数时，对y轴数据做对数
* square root平方根转换：同样适用于数据为正数时，对y轴数据做平方根
* 1/倒数转换：对y轴数据做做倒数
* 数据转换的目的：换一种观察角度；降低偏度；非线性转换为线性
![cars](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eqc9ss266sj20dw07t3z8.jpg)
![cars](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eqc9sta8wxj20dw07twf0.jpg)
![cars](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eqc9sub3ahj20dw07twf5.jpg)


---



#### 1 - 12 - Unit 1, Part 2- (6) Exploring Categorical Variables (8-13) 类别变量

* bar plot柱状图：可以显示类别变量的数量或分布频率。bar plot与his的区别如下图：

![cars](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eqc9sv8d8wj20dw07taar.jpg)

* pie plot饼图：表现的信息量少，尤其是变量多的时候根本无法看出大小的区别。
* contingency table相依表(two Categorical Variables)：按照两个变量将数据列成一个矩阵，这可以用于观察变量之间的相关性

![cars](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eqc9swlqjwj20dw07taay.jpg)

* segmented bar plot分段的柱状图(two Categorical Variables)：在一个变量的柱状图里将另一个变量的分布显示出来（不同的颜色）；relative frequency segmented bar plot相对版本：将条形图的高度调整为频率（同一高度100%）,可以得出相关性。

![cars](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eqc9sxloymj20dw07tt9c.jpg)

* mosaic plot马赛克图(two Categorical Variables)：比相对版本增加了以宽度对应样本数据量的信息（例子同时增加了收入分布的人群分布）

![cars](http://ww2.sinaimg.cn/mw1024/889c2cc9gw1eqc9syn75rj20dw07tjs6.jpg)

* side-by-side box plots(the relationship between a numerical variale and a categorical variable)：观察一个数量变量和类别变量的关系。按照类别变量的分布值分别画出数量变量的箱形图，并排列在一起.

![cars](http://ww1.sinaimg.cn/mw1024/889c2cc9gw1eqc9szlb1lj20dw07tq3g.jpg)

---



#### 1 - 13 - Unit 1, Part 3- Introduction to Inference (12-20) 推断统计学

推断统计学有一套立论逻辑，初学这里很不好理解，多通过具体例子代入是比较好的方式。

以性别歧视为例子来说明，按照性别和是否得到晋升这两个变量画出相依表，可以得到男性得到晋升的百分比，和女性得到晋升的百分比（分别对应男或女总人数计算）。既然我们要来研究性别歧视，我们就要比较这两个百分比的大小，若二者有统计意义上的不同，我们就认为性别歧视是的确存在的。这里的逻辑是先接受一个“平凡”的世界，也就是变量间不存在关系的世界，即：

* **零假设**：待推翻的假设，即现实是不存在性别歧视的，样本中观察到的两个百分比的差异不具有统计意义，性别与是否得到晋升这两个变量是独立的。
零假设是"There is nothing going on"，也就是没有什么特殊的事情发生，相反的：

* **替代假设**：百分比的差异是具有统计意义的，的确存在性别歧视。
接着又举了法庭审判的例子，我觉得这个可以跟“疑罪从无”联系起来。首先默认被告是无罪的，要通过坚实的证据来推翻被告无罪的初始假设，如果证据足够强，则无罪假设被推翻，被告被证明有罪；否则，证据强度不够，法庭无法推翻无罪的初始假设，被告无罪释放。**零假设**：被告无罪；**替代假设**：被告有罪。

也就是说，零假设是个缺省值，在没有信息的基础上，只能接受这个结论。只有仰赖于掌握更多信息来推翻零假设、证明替代假设（或者证明失败）。

后面将对推断统计的具体计算深入讲解。
![cars](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eqc9tdhhynj20dw07t0tj.jpg)
![cars](http://ww3.sinaimg.cn/mw1024/889c2cc9gw1eqc9teexkxj20dw07twfd.jpg)
![cars](http://ww4.sinaimg.cn/mw1024/889c2cc9gw1eqc9tfa9jxj20dw07t0tf.jpg)