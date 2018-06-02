# Comparative-factor-extraction
刘雨薇，南京理工大学，2014级本科

## Table of Contents

- Introduction
- Datasets
- Usage
- Examples
- Note
- Citation

## Introduction

这是我的本科毕业设计(基于机器学习的商品评论要素抽取方法)的代码。

## Datasets

- 比较句语料:COAE2013（第五届中文倾向性评测大会）任务二评测数据
- 比较词候选词典:学姐自己整理的554个比较词候选


## Usage

1.Comparative-factor-extraction-car

   ```latex
  语料库为汽车领域数据
   ```

2.Comparative-factor-extraction-car-multi

   ```latex
  语料库为汽车领域数据中多重比较关系数据
   ```

3.Comparative-factor-extraction-context

   ```latex
  为了验证上下文特征为3时，实验取得最好值
   ```

4.Comparative-factor-extraction-cross

   ```latex
  交叉领域实验，其中测试集为电子领域，训练集为汽车领域
   ```

5.Comparative-factor-extraction-cross2

   ```latex
  交叉领域实验，其中测试集为汽车领域，训练集为电子领域
   ```

6.Comparative-factor-extraction-elec

   ```latex
  语料库为电子领域数据
   ```

7.Comparative-factor-extraction-ner

   ```latex
  为了验证命名实体识别是无效特征
   ```
## Examples

1. 模型训练与学习

   ```latex
   e.g. crf_learn template1.txt trainT1.txt model1
   (根据T1训练数据，训练出了model1模型)
   e.g. crf_test -m model1 testT1.txt >> outputT1.txt
   (根据T1训练好的模型，使用测试集进行测试，并将结果输出到outputT1.txt中)
   ```

## Note

论文中将我的最好数据和COAE2013最大值做了比较，下面是COAE2013任务2.2最大值的数据。

| **比较要素** | **精准评测准确率** | **精准评测召回率** | **精准评测F1值** | **覆盖评测准确率** | **覆盖评测准确率** | **覆盖评测F1值** | 
| ----------- | ---------------: | ---------------: | --------------: | --------------: | ---------------: | :------------: |
|     PROD    |      67.77       |      66.05       |      64.30      |       82.67      |       73.58       |      71.58     |
|     ATTR    |      66.05       |      62.52       |      60.78      |       77.94      |       67.51       |      65.69     |

## Citation

如果您使用此代码，请引用以下文章：

[1] 刘雨薇. 基于机器学习的商品评论要素抽取方法[D]. 南京理工大学, 2018.

更多问题，联系369310624@qq.com
