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
  - [Eigenvalues and equivalent retardance for SLM combinations](#eigenvalues-and-equivalent-retardance-for-slm-combinations)
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

となります.ただしSLM2は光軸に対して $-\frac{\pi}{4}$ 傾いています.つまり

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

に対して $\theta=-\frac{\pi}{4}$ を代入することで得られます.(回転行列で挟んでいます.)

SLMでは偏光分布を,DMで位相分布を変調しています.

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

のように書けます.

</br>

つまり**実験系のジョーンズ行列が分かればその逆行列を作ればよく,作るためには上記3つのパラメーターを調節すれば良い**ということです.

</br>

### Eigenvalues and equivalent retardance for SLM combinations

</br>

SLM1,2がありそれぞれの固有偏光ベクトル,固有値が等しい時,これらを連続してつなげた場合の固有偏光ベクトルと固有値は等しいはずです.この性質を保ったままそれぞれのSLMで偏光状態を変えたいです.

</br>

SLMの場合,x成分の位相のみ変調するのでx成分のみ持つベクトルが固有偏光ベクトルです.また固有値は変調する位相の量です.つまり

</br>

$$
J _ {SLM}:\vec{u} \Rightarrow e^{i\phi}\vec{u} \quad \Bigl(J _ {SLM}=
\begin{bmatrix}
e^{i\phi} & 0 \newline
0 & 1
\end{bmatrix},\vec{u}=
\begin{bmatrix}
x \newline
0
\end{bmatrix}\Bigr)
$$

</br>

という状況です.先ほどの3つのSLMを組み合わせた系を考えます.

</br>

$$
\begin{aligned}
J _ {S}
&=
J _ {SLM3}J _ {SLM2}J _ {SLM1} \newline
&=
a
\end{aligned}
$$

<div style="page-break-before: always;"></div>

## 結果

</br>

<div style="page-break-before: always;"></div>

## 結論

</br>

<div style="page-break-before: always;"></div>