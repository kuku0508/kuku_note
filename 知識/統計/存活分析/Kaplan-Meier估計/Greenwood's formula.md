在估計存活函數的變異數，我們會使用Greenwood's formula。
- - -
# 公式推導：
- 在推導Greenwood's formula之前，需要先認知以下假設
	1. 每個事件時間點的獨立性：
- # 步驟一、計算每個時間點的變異數：
	在每一個時間點$t_i$，事件發生的機率$p_i$ 近似為$\frac{d_i}{n_i}$。根據二項分布的變異數公式，我們可以得到以下公式：
$$
Var(\frac{d_i}{n_i})=\frac{p_i(1-p_i)}{n_i}=\frac{(\frac{d_i}{n_i}-(1-\frac{d_i}{n_i}))}{n_i}
$$
- 