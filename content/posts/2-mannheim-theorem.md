---
title: "2 Mannheim 定理"
date: 2021-02-23T13:39:48+08:00
draft: false
math: true
comment: true
toc: false
---

**Mannheim 定理**　圆 X 与三角形 ABC 的外切圆内切于点 T，且与 AB、AC 相切，切点分别为 P、Q。线段 PQ 的中点即为三角形 ABC 的内心。

![图 2-1][2-1]

**分析**　做好图我们不难猜测四边形 $PBTI$、四边形 $ITCQ$ 都是圆内接四边形，并且两个四边形相似。而证明这一点并不容易。比较自然的想法是通过外角等于内对角来证明，但用这种想法，会发现两个结论相互依赖。因此我们考虑同一法，做出圆 $QCT$，令其交 $PQ$ 于点 $I'$，不难推出另一组共圆，进而证出 $I'$ 和 $I$ 是同一个点。

**证明**　连接 $AX$，交 $PQ$ 于点 $I$，显然 $I$ 是 $PQ$ 的中点。这是因为圆 $X$ 与 $AB$、$AC$ 都相切，因而 $AX$ 平分 $\angle BAC$。又 $AP = AQ$，得出该结论。

设 $\odot ACT$ 交 $PQ$ 于点 $I'$。$I'$ 其实就是点 $I$。下面证实这一点。

（1）四边形 $PBTI'$、四边形 $I'TCQ$ 都是圆内接四边形。

四边形 $I'TCQ$ 是圆内接四边形已经做出。由此及四边形 $ABCT$ 是圆内接四边形知，$\angle TI'Q = \pi - \angle QCT = \angle PBT$，得出四边形 $PBTI'$ 是圆内接四边形。

（2）四边形 $PBTI'$ 与四边形 $I'TCQ$ 相似。

对 $\odot X$ 的切线 $AB$、弦 $PT$ 应用弦切角定理，$\angle BPT= \angle PQT$。又由（1），得 $\triangle PBT \sim \triangle QI'T$。类似地，$\triangle PI'T \sim \triangle QCT$，得出（2）。

由（2）及（1），显然有 $\angle PBI = \angle PTI =\angle QTC$。延长 $TQ$ 交圆 $O$ 于点 $S$ 熟知在这样的图中，$\angle ATS = \angle STC$（对于 $A$、$T$、$P$、$B$ 也是），只要证 $\angle ATS = \angle ABI'$。由此及图形猜测 $B$、$I'$、$S$ 共线，如果猜测正确，两角对应同一个弧，即可得出 $BI'$ 平分 $\angle ABC$。由对称性，对于 $C$ 也有同样的性质，进而 Mannheim 定理成立。

（3）$B$、$I'$、$S$ 三点共线。

由（1），$\angle ABI' = \angle PTI'$。由（4），$\angle PTI' = \angle STC$。熟知 $\angle ATS = \angle STC$，而 $\angle ATS = \angle ABS$，得出 $\angle ABI' = \angle ABS$，即（3）。

证毕。

[2-1]: /images/2-mannheim-theorem.png
