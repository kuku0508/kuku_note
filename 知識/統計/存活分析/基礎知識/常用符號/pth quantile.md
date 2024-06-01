pth quantile，就是指[[Survival Time|存活時間]]的百分位數，以$t_{p}$表示。
- - -
# 備註：
$t_{0.5}=median$
![[median in Survival function.png]]
- - -
# 公式：
$$
t_p=int\
$$
## 連續型：當t為continuous的時候
$$
\begin{align}
&F(t_p)=P(T\leq t)=p\\
&= 1-S(t_p)
\end{align}
$$
![[example F(t)-t圖 in pth quantile.png]]
$$
\begin{align}
\Rightarrow S(t_p)=P(T>t_p)=1-p
\end{align}
$$![[Pasted image 20240602074948.png]]
- - -
