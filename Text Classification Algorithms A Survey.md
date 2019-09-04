# Text Classification Algorithms: A Survey

## Introduction

![](/home/vinnyhu/图片/屏幕截图_1.png)

讲述了文本分类任务，大致上的四个流程：特征提取、降维（可选）、分类算法（最重要的）、效果评估。

然后对每个部分的任务进行了粗略的讲述，论述了本文每一部分的重点内容。

## Text Preprocessing

###　Text Cleaning and Pre-processing

这一部分其实就是相当于对数据进行清洗，但是在看一些文本分类的比赛中，很多词都是脱敏的，所以这一步貌似是不需要做的有时候。

*　词干化。
*　去除停用词
*　大小写转化
*　俚语和缩写处理
*　去除噪声　如去除标点符号、特殊字符等
*　拼写纠错
*　提取词干，提取词根，比如study、studying，表达的意思是一样的

### Syntactic Word Representation（句法词表示）

这一步其实就相当于是特征抽取部分，这部分的研究是相当多的，像词袋模型、向量空间模型、矩阵分解、主题模型、到现在非常火的用各种RNN、CNN、attention等深度学习做的，本质上都相当于是特征抽取器。之前自己也看过不少这一点的东西，但是还是看的太浅，数量太少，以后还是要花大力气好好看看学习学习。

* N-Gram    “The n-gram technique is a set of n-word which occurs “in that order” in a text set. This is not a representation of a text, but it could be used as a feature to represent a text.”这句话说的非常好，一语点出了N-Gram的实质。

### Weighted Words（权重词表示）

最常用的还是当属TF-IDF了

* BOW 模型，大概讲解了BOW的思想、限制等。
* TF-IDF  大致讲了怎么计算的，这方面就不用怎么看了，关于tfidf的博客介绍等太多了，又说了一下缺点，就是无法计算词义相似性问题。

### Word Embedding （词嵌入）

这里面介绍的每种词嵌入方法都值得深究，后续仔细看paper，然后再写博客去研究。

* Word2vec
* Global Vectors for Word Representation (GloVe)
* FastText
* Contextualized Word Representations
* 



