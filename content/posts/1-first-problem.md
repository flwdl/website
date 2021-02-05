---
title: "1 首题"
date: 2021-02-15T19:00:00+08:00
draft: false
math: true
---

这大概是我独立做出的第一道比较复杂的（至少看起来是这样）竞赛平面几何题（泪目）。

![图 1-1][1-1]

如图，过 $\triangle ABC$ 的内心 $I$ 的直线交 $\triangle ABC$ 的外接圆于 $Q$、$P$。$AP$ 交 $BC$ 于点 $E$，$Q$ 交 $BC$ 于 点 $F$。求证：$A$、$I$、$E$、$F$ 四点共圆。

![图 1-2][1-2]

**证明：** 如图，连接 $AI$ 并延长至外接圆上的点 $S$，设 $AS$ 交 $BC$ 于点 $U$。由 $AS$ 平分 $\angle BAC$ 及 $S$、$A$、$B$、$C$ 共圆，

<div>
$$
\begin{aligned}
\angle SUC &= \angle SAC + \angle BCA \\
           &= \angle SAB + \angle BCA \\
           &= \angle SCB + \angle BCA \\
           &= \angle SCA.
\end{aligned}
$$
</div>

由此得到 $\triangle SUC \sim \triangle SCA$，得 $SI^2 = SC^2 = SU \cdot SA$（第一个等号可由熟知的「鸡爪定理」得到）。

希望再找到一个像 $SU \cdot SA$ 的量，由此可以确定一些圆内接四边形，对目标有所帮助。

还是利用 $\angle SUC = \angle SCA$。结合 $\angle SCA = \angle SPA$，不难想到在远处 $SP$ 与 $BC$ 有一交点 $T$，显然有 $\triangle SUT \sim \triangle SUA$，得到 $A$、$U$、$P$、$T$ 四点共圆。

由圆幂定理，$SP \cdot ST = SU \cdot SA$。那 $SI^2$ 也 $= SP \cdot ST$，这样，$\triangle SPI \sim \triangle SIT$。注意，

<div>
$$
\begin{aligned}
(\angle SAP + \angle API &=) \angle SIP \\
                         &= \angle STI \\
                        (&= \angle STU + \angle ITU),
\end{aligned}
$$
</div>

而 $\angle SAP = \angle STU$，那 $\angle API = \angle ITU$。设 $AP$ 交 $IT$ 于点 $X$，则 $X$、$U$、$P$、$T$ 四点共圆。由 $TY \perp IP$，$PX \perp IT$，$E$ 为 $\triangle PIT$ 的垂心。

$E$ 为垂心，$IT \perp PT$，$TE \perp IP$，知 $\angle PIE = \angle PTE$，进而 $\angle PIE = \angle PTE = \angle PAI$。我们希望

<div>
$$
\begin{aligned}
(\frac{\pi}{2} - \angle PIE &= )\angle IEB \\
                            &= \angle IAF \\
                           (&= \angle PAI + \angle EAF)
\end{aligned}
$$
</div>

即证 $\angle SOP + \angle EAF = \dfrac{\pi}{2}$。

由于 $OP \parallel PQ$，$\angle SOP = \angle OPQ$。由外心性质（$\angle OPQ + \angle QBP = \dfrac{\pi}{2}$），那么 $\angle SOP + \angle EAF = \dfrac{\pi}{2}$ 等价于 $\angle EAF = \angle QBP$。加之我们有，

<div>
$$
\begin{aligned}
\angle QBP &= \angle QBA + \angle ABC + \angle CBP, \\
\angle EAF &= \angle EAC + \angle CAF, \\
\angle CBP &= \angle CAP = \angle EAC.
\end{aligned}
$$
</div>

于是

<div>
$$
\begin{aligned}
                &\angle EAF = \angle QBP \\
\Leftrightarrow	&(\angle QBA + \angle ABC = ) \angle QBC = \angle CAF \\
\Leftrightarrow	&\frac{\pi}{2} - \angle BQP = \pi - \angle QAC \\
\Leftrightarrow	&\angle QAC - \angle BQP = \frac{\pi}{2} \\
\Leftrightarrow	&\angle QAC - \angle BAP = \frac{\pi}{2} \\
\Leftrightarrow	&\angle QAB + \angle PAC = \frac{\pi}{2}
\end{aligned}
$$
</div>

$\angle QAB + \angle PAC = \dfrac{\pi}{2}$ 是显然的。

<p style="text-align: right">$\text{Q.E.D.}$</p>

[1-1]: /images/1-first-problem-img1.png
[1-2]: /images/1-first-problem-img2.png
