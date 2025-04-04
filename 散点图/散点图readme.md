# 回归分析可视化工具 (R Script)

## 简介
这是一个基于R语言的交互式脚本，用于快速生成带有回归方程和统计信息的散点图。脚本会引导用户输入数据，自动计算回归模型，并生成专业美观的可视化图表。

## 功能特点
- 交互式数据输入（支持中英文）
- 自动计算回归方程和R²值
- 智能坐标轴刻度调整
- 支持中文标题和标签
- 自动保存图表为PNG格式
- 专业学术图表风格
## 例图
<a href="https://github.com/Chinaduanyun/R_Learning-Develop/blob/main/散点图/例图.png">
  <img src="https://raw.githubusercontent.com/Chinaduanyun/R_Learning-Develop/main/散点图/例图.png" width="300" alt="icon"/>
</a>


## 使用说明

### 1. 系统要求
- R (≥ 3.6.0)
- 以下R包：
  - ggplot2
  - ggthemes
  - showtext
  - ggpmisc

### 2. 安装依赖
```r
install.packages(c("ggplot2", "ggthemes", "showtext", "ggpmisc"))
```

### 3. 运行脚本
1. 将脚本保存为`regression_plot.R`
2. 在R中运行：
```r
source("regression_plot.R")
```

### 4. 交互式输入
脚本会依次提示输入：
- X轴标题
- X轴数据（英文逗号分隔）
- Y轴标题
- Y轴数据（英文逗号分隔）
- 图表标题（可选）

### 5. 输出结果
- 自动显示图表
- 自动保存为PNG文件（格式：pic_YYYYMMDD_HHMMSS.png）

## 示例输入
```
请输入X轴标题：
实验组别
请输入X轴数据（英文逗号分隔）：
1,2,3,4,5
请输入Y轴标题：
测试得分
请输入Y轴数据（英文逗号分隔）：
65,78,82,88,95
请输入图表标题（可选，直接按Enter跳过）：
实验组别与测试得分关系
```

## 输出示例
生成的图表包含：
- 散点图
- 回归线
- 回归方程（格式：y = a + bx）
- R²值
- 自动优化的坐标轴

## 自定义选项
用户可以直接修改脚本中的以下参数：
- 点样式（颜色、大小、形状）
- 回归线样式
- 字体设置
- 图表尺寸和分辨率

## 注意事项
1. 确保中文字体路径正确==（脚本默认使用Mac系统的宋体）==
2. 数据输入时请使用英文逗号分隔
3. 图表会自动保存到当前工作目录
