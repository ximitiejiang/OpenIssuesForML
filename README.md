# OpenIssuesForML

record machine learning algorithm open issues and answers

# Q_数据处理：如何处理特征向量的缺失值？
特征向量缺失值处理方法有如下几种：
## 1）缺失值较多：
    超过20%，则考虑直接舍弃该特征
## 2）缺失值较少：
    - 用0值填充
        ```python
        train.fillna(0)
        ```
    - 用平均值填充
    - 用众数填充
    - 用插值法填充
    - 用随机森林法预测：
        > 将数据分为有值和缺失值2份，对有值的数据采用随机森林拟合，然后对有缺失值的数据进行预测，用预测的值来填充。



# Q_