mean residual life(平均餘命)，又被稱為Expected Remaining Lifetime。是指在時間點t之後，個體沒有發生事件的條件下，剩餘存活期間的期望值。
- - -
# 公式：
$$
\begin{align}
m(t)
=&E\left[T-t\mid T>t \right]\\
=&\int^\infty_t(u-t)f(u\mid T>t)du\\
=&\int^\infty_t(u-t)\frac{f(u)}{P(T>t)}\\
=&\int^\infty_t(u-t)\frac{f(u)}{S(t)}\\
=&\frac{\int^\infty_t(u-t)f(u)du}{S(t)}\\
=&\frac{\int^\infty_tuf(u)-tf(u) \,du}{}
\end{align}
$$