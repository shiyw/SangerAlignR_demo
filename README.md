# SangerAlignR Demo

## 介绍
SangerAlignR 遗传性疾病sanger测序验证便捷查看。
此处为SangerAlignR的使用介绍

## 使用
### 依赖
可以使用renv来管理依赖，也可以手动安装

#### renv
```bash
git clone https://github.com/shiyw/SangerAlignR_demo.git
cd SangerAlignR_demo
```

```r
if (!requireNamespace("renv", quietly = TRUE)) {
  install.packages("renv")
}
renv::restore()
```

#### 手动安装
```r
install.packages("pak")
pak::pak(c("tinytex", "tidyverse", "shiny", "knitr", "Biostrings", "msa", "msaR", "sangerseqR",
          "devtools", "DECIPHER", "RUnit", "tinytex"))
tinytex::install_tinytex()
```

### 安装SangerAlignR
```r
pak::pak("shiyw/SangerAlignR")
```

### 打开ShinyAPP
```r
SangerAlignR::PolyPeakParser()
```

