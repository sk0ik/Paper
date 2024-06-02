<div style="text-align: center; font-size: 25px; font-weight: bold;">
title
</div>

</br>

- [概要](#概要)
- [研究背景](#研究背景)
- [研究目的](#研究目的)
- [原理](#原理)
  - [SLMs+DM](#slmsdm)
  - [Elliptical retarder](#elliptical-retarder)
- [結果](#結果)
- [結論](#結論)


</br>

## 概要

</br>

- a
- b
- c

</br>

<div style="page-break-before: always;"></div>

## 研究背景

</br>

こう言う技術があってこういう分野で使われている

<div style="page-break-before: always;"></div>

## 研究目的

</br>

現状の課題を解決するためなど

<div style="page-break-before: always;"></div>

## 原理

</br>

### SLMs+DM

</br>

論文中で使用しているSLM3個,Deformable Mirror1個で変調する場合,ジョーンズ行列はそれぞれ

</br>

$$
\begin{aligned}
J _ {SLM1}
&=
\begin{bmatrix}
e^{i\psi _ 1} & 0 \newline
0 & 1
\end{bmatrix} \newline
J _ {SLM2}
&=
\frac{1}{2}
\begin{bmatrix}
e^{i\psi _ 2}+1 & e^{i\psi _ 2}-1 \newline
e^{i\psi _ 2}-1 & e^{i\psi _ 2}+1
\end{bmatrix} \newline
J _ {SLM3}
&=
\begin{bmatrix}
e^{i\psi _ 3} & 0 \newline
0 & 1
\end{bmatrix} \newline
J _ {DM}
&=
e^{i\psi _ {DM}}
\begin{bmatrix}
1 & 0 \newline
0 & 1
\end{bmatrix}
\end{aligned}
$$

</br>

となる.ただしSLMは光軸に対して $-\frac{\pi}{4}$ 傾いている.つまり

</br>

$$
J _ {SLM2}=
\begin{bmatrix}
\cos{\theta} & \sin{\theta} \newline
-\sin{\theta} & \cos{\theta}
\end{bmatrix}
\begin{bmatrix}
e^{i\psi _ 2} & 0 \newline
0 & 1
\end{bmatrix}
\begin{bmatrix}
\cos{\theta} & -\sin{\theta} \newline
\sin{\theta} & \cos{\theta}
\end{bmatrix}
$$

</br>

に対して $\theta=-\frac{\pi}{4}$ を代入することで得られる.

SLMでは偏光分布を,DMで位相分布を変調している.

</br>

### Elliptical retarder

</br>

ジョーンズ行列を一般化すると

</br>

$$
J _ {E}=e^{-i\frac{\phi}{2}}
\begin{bmatrix}
\cos^2{\theta}+e^{i\phi}\sin^2{\theta} & (1-e^{i\phi})e^{-i\alpha}\sin{\theta}\cos{\theta} \newline
(1-e^{i\phi})e^{i\alpha}\sin{\theta}\cos{\theta} & \sin^2{\theta}+e^{i\phi}\cos^2{\theta}
\end{bmatrix}
$$

- $\theta:\text{orientation}$
- $\phi:\text{retardance}$
- $\alpha:\text{parameter(determines the ellipticity of the eigenstate)}$

</br>



<div style="page-break-before: always;"></div>

## 結果

</br>

<div style="page-break-before: always;"></div>

## 結論

</br>

<div style="page-break-before: always;"></div>