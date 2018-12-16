# 课程作业

## [一. Hadoop分布式环境安装](https://gitlab.chpengzh.com/chpengzh/big-data-course/tree/master/doc/project0)

要求：

完成Hadoop分布式环境的搭建，并实现课上讲的baseline和in-mapper-combine的word count程序。输出结果按字典序排序。

回答问题：

- 1.结果中出现在第1个位置的单词是什么，word count的结果是多少？
- 2.结果中出现在第10个位置的单词是什么，word count的结果是多少？
- 3.比对baseline和in-mapper-combine的程序分别执行时间

## [二. MapReduce程序实验](https://gitlab.chpengzh.com/chpengzh/big-data-course/tree/master/doc/project1)

要求：

完成计算PMI互信息的MapReduce，计算语料库中两两单词的互信息，分别使用pair和stripes两种数据结构。并且要求在使用combiners的情况下完成实验。

```math
PMI(x,y)=\log {\frac{p(x,y)}{p(x)p(y)}}
```

回答问题：

- 1.对比使用combiners和不适用combiners时，完成pair和stripes两种数据结构的程序所用的时间？
- 2.最终计算结果中包含多少个不同的PMI值？
- 3.具有最高PMI值的单词组是什么？PMI值是多少？

## [三. 倒排索引建立](https://gitlab.chpengzh.com/chpengzh/big-data-course/tree/master/doc/project2)

要求：

在Hadoop分布式环境中实现课上讲的对语料库构建倒排索引的程序（可选项：对倒排索引进行压缩。完成可选项有附加分）。
      
回答问题：

- 1.计算结果中一共有多少个索引？
- 2.哪个单词具有最长的索引项？
- 3.可选项：对比原始索引和压缩索引分别需要的计算时间，以及计算结果占有的存储空间。

## [四. 用户权值计算](https://gitlab.chpengzh.com/chpengzh/big-data-course/tree/master/doc/project3)

要求:

分别在Hadoop和Spark平台上实现微博用户重要度排序。以通过计算用户的PageRank值实现，其它任选方法也可以

提交一个报告，包括5个部分：

- 实验环境部署
- 方法介绍
- 实验结果统计
- 对两个平台上实现方法的对比（包括：程序的对比、数据加载时间、第一轮迭代用时、每轮迭代的平均时间、总的算法执行时间等）