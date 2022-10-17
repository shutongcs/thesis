# thesis

## 字体
- 加粗黑体用SimHei、加粗楷体用STKaiti、加粗宋体用SimSun
- 用AutoFakeBold={}指定加粗的程度，可以用来做微调，但是由于是autofakebold，难以做得跟windows版本的一模一样

## 排版
### 目录
- 目录生成后要用acrobat把中英文摘要页数的括号去掉
- 目录标题和目录间的距离默认是\addtocontents{toc}{\vspace{5pt}}，但因为latex的@#$&^$%&的规定，我的第四章全都被放到第二页，导致目录第一页有很大的空白。如果本身不存在这样的问题的话，可以在cls文件里改回默认值，否则要用vspace调一下

### 图表
- 图中文本渲染错误出现异常的解决方式[[link](https://github.com/mohuangrui/ucasthesis/wiki/%E5%AD%97%E4%BD%93%E9%85%8D%E7%BD%AE#%E5%9B%BE%E4%B8%AD%E6%96%87%E6%9C%AC%E6%B8%B2%E6%9F%93%E9%94%99%E8%AF%AF%E5%87%BA%E7%8E%B0%E5%BC%82%E5%B8%B8%E5%8A%A0%E7%B2%97)]

### 算法
- 解决算法标题字号小的问题：在\begin{algorithm}后，\caption之前加入一行\captionsetup{font=normalsize}

