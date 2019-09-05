# introduction-to-algorithm
# 概率分析和随机算法

## 雇用问题

**概率分析：**我们对所有可能输入产生的运行时间取平均。当报告此种类型的运行时间时，我们称其为平均情况运行时间。

## 指示器随机变量



# 中位数和顺序统计量

第$$i$$个顺序统计量是该集合中第$$i$$小的元素。最小值是第1个顺序统计量，最大值是第$$n$$个顺序统计量。

本章将讨论从一个由$$n$$个互异的元素构成的集合中选择第$$i$$个顺序统计量的问题。

## 最小值和最大值

同时找到最小值和最大值，下面有两种方式，第二种方式更优：

- 分别独立的找出最小值和最大值，这各需要$$n-1$$次比较，共需$$2n-2$$次比较。
- 记录已知的最小值和最大值，但我们并不是将每一个输入元素与当前的最小值和最大值进行比较，而是对输入元素成对的进行处理。首先，我们将一对输入进行相互比较，然后将较小的与当前最小值进行比较，把较大的与当前最大值进行比较。这样，对每两个元素需$$3$$次比较，所以总共需要$$3\left \lfloor \frac{n}{2} \right \rfloor$$ 次比较。

## 期望为线性时间的选择算法

