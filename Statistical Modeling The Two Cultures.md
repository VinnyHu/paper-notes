# Statistical Modeling: The Two Cultures

读这篇论文是因为前段时间在一个公众号上面看到一个人对这篇论文的评价和理解，当时感觉这篇论文挺好的，虽然很早就下载下来了，但是今天才来打开仔细阅读。但是由于这篇论文是2001年时候写的，所以论文中的观点比如对于统计学界大家的工作方式之类的可能在今天就不太适应了，毕竟科学发展日新月异，2001年对于计算机、机器学习这种学科来讲可能是上古时代了，不过我还是想读一下这篇论文，里面有的思想应该还是挺好的。阅读了一部分之后感觉不太对劲，后来看了仔细看了作者才发现，原来这是个发明决策树算法的大佬！

##　摘要

首先说明了统计学中一般有两种想法，①假设数据是由一个随机分布生成的（在ML中有许多的算法都是基于此类假设的）。②用算法模型，并且假设对于数据的产生机制是未知的。作者认为在统计学界前一种思维方式被非常广泛的采用，这导致了很多的问题，实际上后一种方式是非常有用的，不管对于大数据还是小数据的处理，后一种方式都有非常多的优势。

## 导论

写的非常清晰易懂，介绍了两种方法的工作思路。

首先定义问题：对于很多问题我 们都可以假定为如下的方式，x表示预测变量，y表示响应变量。黑箱表示一个未知的函数，这个函数对预测变量进行某种操作然后生产了响应变量。

![](/home/vinnyhu/图片/屏幕截图_18.png)

最终有两个目标：①由新来的x，我们想要生产对应的y。②了解那个黑箱，知道x和y之间的关系。

###  The Data Modeling Culture

此种方法首先对黑箱假设成某一个随机的数据模型，例如如下所示：


![](/home/vinnyhu/图片/屏幕截图_19.png)

参数都由数据来估计，生成的模型接下来就可以进行预测了。

![](/home/vinnyhu/图片/屏幕截图_20.png)

最后大概就是这种样子，身边有一大类的算法都是这样的，而且作者认为98%的统计学家都是按照这种方式来工作的。其实刚接触机器学习时，大家接触的更多的也是这种算法。

### The Algorithmic Modeling Culture

这种方法假设黑箱是复杂的、未知的。他的方法就是去找到一个f(x) 可以很好的预测y。

![](/home/vinnyhu/图片/屏幕截图_21.png)

上面提到了神经网络和决策树，神经网络根据万能逼近定律可以无限的逼近任意的连续函数，不过其黑盒性质还是被很多人诟病的，现在已经有很多学者投入相关研究了，以后可以根据课程学习一下。

其实作者是站The Algorithmic Modeling Culture 这种方法的队，在文中会批评前一种方法。

## ROAD MAP

这一章就是介绍一下论文的大致结构。

## PROJECTS IN CONSULTING

这里就是介绍一下之前作者职业生涯中参与过的项目

#### The Ozone Project

都是讲述他的一些项目经历而已

#### Perceptions on Statistical Analysis

这里是聊他的收获：a专注于寻找一个好的解决方法，这是咨询员的职责所在。b在你寻找模型之前，先专注与数据。c寻找一个可以给出好的方法的模型。d在测试集上面的变现结果是对模型好坏的评价指标。e计算机是不可或缺的搭档

## THE USE OF DATA MODELS

这里其实就是对于data model的描述和他们局限性的指出。

未完待续。。。