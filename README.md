# MLE
NBA2018-2019赛季MVP评选即将见分晓，预测MVP是一件非常有趣的事情。可把MVP预测看作一个二分类问题：是MVP或者不是MVP。于是可选用一些常见的分类模型。
在这使用logistic回归进行建模，利用历史数据对2018年和2019年MVP进行预测。

1.数据来源：kaggle 和 basketball reference
2.数据准备：1956-2007年数据作训练集，其中特征数有25个（['G', 'GS', 'MP',
       'FG', 'FGA', 'FG%', '3P', '3PA', '3P%', '2P', '2PA', '2P%', 'eFG%',
       'FT', 'FTA', 'FT%', 'ORB', 'DRB', 'TRB', 'AST', 'STL', 'BLK', 'TOV',
       'PF', 'PTS']），训练标签为({1:MVP, 0:not MVP) . 2008-2017作预测集. 
       
3.模型：logistic二分类器 
  Loss function: 交叉熵 
  优化：Adam随机梯度法 
  
4.训练结果：Epoch:10000,Loss:0.3210,Accuracy：0.9931.
  预测结果：
 【2018年】 
Anthony Davis
Kevin Durant
James Harden（MVP）
Jrue Holiday
LeBron James
Karl-Anthony Towns
Jacob Wiley

【2019年】
Ryan Anderson,
Giannis Antetokounmpo,
Stephen Curry,
Kevin Durant,
Pau Gasol,
James Harden,
Alize Johnson,
Zhaire Smith,
Nikola Vucevic,








           
