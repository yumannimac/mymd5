<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>

<script type="text/javascript" async="" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>


# バーゼル問題
バーゼル問題を解く。すなわち

$$
S=\lim_{n \to \infty }\sum_{k=1}^{n} \frac{1}{k^2}=\frac{\pi ^2}{6} 
$$

の証明をする。

## 証明
$\mathbb{R}^2$において$C^2$級の関数を考える。これはフーリエ級数展開できる。
$C^2$級の関数の例を考える。

$$
f \left(x\right) =x^2
$$

は$C^2$級である。なぜなら

$$
f'\left(x\right) =2x
$$


$$
f''\left(x\right) =2
$$

となり確かに存在するからである。
ところで

$$
f \left(x\right) =x^2=\sum_{n=0}^{\infty } a_n \cos nx
$$

と表すことができると仮定しよう。

$$
\int_{-\pi }^{\pi } x^2 \cos nx dx= \left[ \frac{1}{n}x^2 \sin nx+\frac{1}{n^2}\cdot 2x \cos nx +\frac{1}{n^3}2 \sin nx \right]_{-\pi }^{\pi }=\left(-1\right) ^n\frac{4 \pi }{n^2}
$$

であるから

$$
f \left(x\right) = x^2=\frac{\pi ^2}{3}+4\sum_{n=1}^{\infty} \frac{\left(-1\right) ^n}{n^2}\cos nx
$$

と考えられる。
したがって

$$
f \left(0\right) =0=\frac{\pi ^2}{3}+4\sum_{n=1}^{\infty} \frac{\left(-1\right) ^n}{n^2}
$$

より

$$
\sum_{n=1}^{\infty } \frac{\left(-1\right) ^n}{n^2}
=-\frac{\pi ^2}{12}
$$

である。

$$
\begin{split}
  \sum_{n=1}^{\infty } \frac{\left(-1\right) ^n}{n^2}
  &=\, 
-\frac{1}{1^2}+\frac{1}{2^2}-\frac{1}{3^2}+\frac{1}{4^2}+\dots \\
&=\, -\left(\frac{1}{1^2}+\frac{1}{2^2}+\frac{1}{3^2}+\dots\right) +2 \left(\frac{1}{2^2}+\frac{1}{4^2}+\dots\right) \\
&=\, -S+\frac{1}{2}\left(\frac{1}{1^2}+\frac{1}{2^2}+\frac{1}{3^2}+\dots\right) \\
&=\, -\frac{S}{2}
\end{split}
$$

であるから

$$
S=\sum_{n=1}^{\infty } \frac{1}{n^2}=\frac{\pi ^2}{6}
$$

が示された。$\square$


$$
\newcommand{\alk}{\alpha}
$$

$$
\alk+
$$

$$
    \gdef\mysquare#1{#1^2}
    % \newcommand\mysquare[1]{#1^2}
    \gdef\setcomp#1#2{\left\{#1\mid#2\right\}}
$$

グローバルにマクロが定義されているので, $\mysquare{x}$ や $\mysquare{(ab)}$ のようにインライン数式でも

$$ 
S^1 = \setcomp{(x, y) \in \mysquare{\R}}{\mysquare{x} + \mysquare{y} = 1} 
$$

のようにディスプレイ数式でもどこからでも利用できる.

$alk$
