# 中研院生醫所學術專題: 癌症病人存活預測

### 主要參考論文 : 
> [Assessing the clinical utility of cancer genomic and
proteomic data across tumor types](https://www.nature.com/articles/nbt.2940.pdf)

>[Predicting clinical outcomes from large scale cancer genomic profiles with deep survival models](https://www.nature.com/articles/s41598-017-11817-6)

***

# 準備:

### 環境為 Anaconda 底下的 Jupyter notebook

### 1.install plotly 

```
##繪圖用的library
conda install -c plotly plotly
```

### 2.使Jupyter Notebook中能單獨開啟並執行R文件
![run R on jupyter notebook](https://i.imgur.com/GQAlIRn.png)

```
## 安裝完之後可以在jupyter notebook中單獨開啟執行R的文件
conda install -c r r-essentials
```
> 雖然在jupyter notebook中的python文件內能夠使用 
> > %load_ext rpy2.ipython 
> > 
> > %R install.packages("R_package")
> 
> 指令呼叫R的來使用，但是在安裝第三方Library上容易出錯，所以在這裡我選擇另外開啟一個R文件，事先將R會用到的Library先安裝好。

---

# 如何使用:

### 1.將 load_R.ipynb、main.ipynb放在與Data資料夾同一層下，如下圖
![structure](https://i.imgur.com/QTcE4Uy.png)

### 2.第一次使用先執行 load_R.ipynb

>**load_R.ipynb** => 如果第一次使用，需先執行此檔案，因main.ipynb內會呼叫R的library，執行此程式將未下載的R的library安裝好。

### 3.執行主程式 main.ipynb
>**main.ipynb** => 資料切割、呼叫R的library、利用論文內的方法算出c-index、使用plotly作圖

---


