# NLP


赛题：零基础入门NLP之新闻文本分类（赛题理解）

一、赛题背景：根据新闻文本字符对新闻的类别进行分类，属于文本分类问题； 

二、赛题数据：新闻文本，并按照字符级别进行匿名处理。整合划分出14个候选分类类别：财经、彩票、房产、股票、家居、教育、科技、社会、时尚、时政、体育、星座、游戏、娱乐的文本数据。 赛题数据由以下几个部分构成：训练集20w条样本，测试集A包括5w条样本，测试集B包括5w条样本。为了预防选手人工标注测试集的情况，数据的文本按照字符级别进行了匿名处理。 

三、评测指标：评价标准为类别f1_score的均值，结果越大越好。 计算公式：F1=2∗(precision∗recall)(precision+recall) 

四、数据读取：使用pandas对数据进行读取并进行数据分析 

五、解题思路： 本题难点在于对匿名字符进行建模，建模过程涉及到两个过程：特征选取+分类模型 思路1：TF-IDF+机器学习分类器 思路2：FastText 思路3：WordVec+深度学习分类器 思路4：Bert分类器
