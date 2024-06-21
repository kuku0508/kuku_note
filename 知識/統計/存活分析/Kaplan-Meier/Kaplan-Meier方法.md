Kaplan-Meier方法，也被稱為Product Limit方法，是一種無母數估計方法。Kaplan-Meier方法不是將時間分群成區間，而是用到每個個體確實存活時間的無母數技巧。而Kaplan-Meier方法能夠用於具有設限情況的存活資料。
- - -
# 公式：
$$
\begin{align}
S(t_j)&=S(t_{j-1})P(T>t_j\mid T>t_{j-1})\\
&=\prod_{i=1}^jP(T>t_i\mid T>t_{i-1})=\prod^j_{i=1}(1-\frac{d_i}{n_i})=\prod^j_{i=1}(\frac{n_i-d_i}{n_i})
\end{align}
$$
上面那一行是KM公式，下面那一行是Product Limit公式
- - -
# 應用：
40歲前曾做HIV血清轉換的12名樣本血友病患者被診斷出得AIDS