# 函數說明：
- ## boot：
``` R
boot(data,statistic,R,sim="ordinary",stype="i",strata = NULL,...)
```
### 參數：
- `data`：原始資料集。
- `statistic`： 用於計算統計量的函數。這個函數應該接受兩個參數：原始數據和一個索引向量，並返回一個統計量值。
- `R`：重抽樣次數。
- `sim`：模擬類型。默認為 "ordinary"（普通的 Bootstrap），其他選項包括 "balanced"（平衡 Bootstrap）等。
- `stype`：樣本類型。默認為 "i"，表示使用索引。
- `strata`： 分層變量，用於分層抽樣。
- `...`： 傳遞給 `statistic` 函數的其他參數。

- ## boot.ci：
``` R
boot.ci(boot.out, conf = 0.95, type = c("norm", "basic", "stud", "perc", "bca"), ...)
```

### 參數：

- `boot.out`: 由 boot 函數生成的 Bootstrap 結果。
- `conf`: 信心水準。默認為 0.95。
- `type`: 要計算的信賴區間類型。可以是 "norm"（常態法）、"basic"（基本 Bootstrap）、"stud"（學生化 Bootstrap）、"perc"（百分位法）、"bca"（BCa Bootstrap）等。
- `...`: 其他參數。
- - -
# 
- - -
parent::[[Bootstrap Confidence Interval]],[[R語言目錄]]