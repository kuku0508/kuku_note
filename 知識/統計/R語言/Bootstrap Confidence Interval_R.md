``` R
# 安裝並載入所需的包
install.packages("boot")
library(boot)

# 創建樣本資料集
data <- c(2, 4, 5, 7, 9)

# 定義計算平均值的函數
mean_function <- function(data, indices) {
  return(mean(data[indices]))
}

# 設定重抽樣次數
B <- 1000

# 使用boot函數進行Bootstrap
bootstrap_results <- boot(data, statistic = mean_function, R = B)

# 設定信心水準
confidence_level <- 0.95

# 使用boot.ci函數計算信賴區間
confidence_interval <- boot.ci(bootstrap_results, type = "perc", conf = confidence_level)

# 輸出結果
print(bootstrap_results)
print(confidence_interval)
```
