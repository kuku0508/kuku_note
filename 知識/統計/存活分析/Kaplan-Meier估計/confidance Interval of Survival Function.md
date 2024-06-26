當我們今天得到了[[Greenwood's formula|存活函數的變異數]]後，我們就可以透過變異數來去估算[[Survival Function|存活函數]]的信賴區間。而估算方法如下：
- - -
# 公式：
- # 方法一：普通信賴區間方法(Standard Confidence Interval Method)
這個方法就直接使用標準的方法來估算信賴區間，用的就是以下公式
$$
\hat{S}(t)\pm z_{\frac{a}{2}}\times\hat{\sigma}(t)
$$
- # 方法二：對數變換方法(Log-Transformation Method)
1. 計算對數存活函數的標準誤：
$$
\hat{\sigma}_{log}(t)=\frac{\hat{\sigma}(t)}{\hat{S}(t)}
$$
2. 計算對數存活函數的信賴區間：
$$
log(\hat{S}(t))\pm z_{\frac{a}{2}}\times \hat{\sigma}_{log}(t)
$$
3. 反對數變換，得到存活函數的信賴區間：
$$
\left( exp(log(\hat{S}(t))-z_{\frac{a}{2}}\times \hat{\sigma}_{log}(t))\right ) ,\left( exp(log(\hat{S}(t))+z_{\frac{a}{2}}\times \hat{\sigma}_{log}(t))\right ) 
$$
- - -
parent::[[Greenwood's formula]],[[Survival Function]],[[存活分析目錄]],[[信賴區間]]