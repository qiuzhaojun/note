

## numpy

|      |                        |
| ---- | ---------------------- |
|      | np.logspace(0,2,num=5) |
|      |                        |
|      |                        |
|      |                        |
|      |                        |



## pandas

| 解释 | 函数 |
| :------------: | :--------------------: |
| 列中值统一减去 | dataframe.col2 - value |
| 绝对值、平均值 | dataframe.col.**abs( )**           **mean()** |
| 统计数值个数 | dataframe.col.**value_counts( )** |
| 列中值相减 | dataframe.col1 - dataframe.col2 |
| 排序 | dataframe.col.**sort_index( )** |
| 随机选择数据、洗牌 | dataframe.**sample( )** |
| 替换 | dataframe.col.**replace**("/"," ") |
| 切片 | dataframe.col.**iloc**[ : ] |
| 删除行/列 | dataframe.**drop**( "col", axis=1) |
| 调用函数 | dataframe.col.apply( ) |
|      表格形状      |              dataframe.**shape**              |
|     返回非空值的series     | pandas.**notnull**(dataframe.col) |
| 列出列表中不同值 | dataframe.col.**unique( )** |
| 调用函数 | dataframe.col.**apply**(lambda x: x.split(",")) |
| 分组函数 | dataframe.**groupby**(col) |
| 聚合函数 | dataframe.**groupby**(col).**agg**({'col2':"median",'col3':"mean"}) |
| transfrom聚合函数 | data['avg_salary'] = data.groupby('company')['salary'].**transform**('mean') |
| one-hot编码 | pandas.**get_dummies**(dataframe.col,prefix="...") |
| 指标统计 | dataframe.**describe()** |
|  |  |
|  |  |



## matplotlib

|      解释      |                     函数                      |
| :------------: | :-------------------------------------------: |
|  导入pylot包   |        import matplotlib.pylot as plt         |
|  定义画图函数  |        plt.figure(figuresize=(10,10))         |
|    定义多图    | plt.subplot(121)    1*2的图，其中这是第一张图 |
|  设置图片标题  |              plt.title("title")               |
|    画散点图    |         plt.scatter(x,y,color='red')          |
| 设置坐标轴名称 |            plt.xlabel("new name")             |
|                |                                               |
|                |                                               |
|                |                                               |



## 类型

|          解释          | 函数      |
| :--------------------: | --------- |
|   返回参数的数据类型   | type( )   |
| 返回数组中元素数据类型 | .dtype    |
|   对数据类型进行转换   | astype( ) |
|                        |           |



## sklearn

|              |                                                              |
| ------------ | :----------------------------------------------------------: |
| 标准化       |       standardscaler( ).fit_transform(dataframe[col])        |
| 计算距离     | from scipy.spatial import distance<br/>distance.euclidean(list1,list2) |
| 交叉验证     | from sklearn.model_selection import KFold<br />KFold = **KFold**(len,n_splits=5,shuffle=True)<br />for train_index,test_index in **KFold.split**(datafram):<br />返回表格索引值index,type=ndarray |
| 随机森林分类 | from sklearn.ensemble import RandomForestClassifier<br />**RandomForestClassifier**(n_estimators=n,max_depth=m) |
|              |                                                              |



## 面向对象

|        |              |
| :----: | ------------ |
| 类对象 | @classmethod |
|        |              |
|        |              |



## IO

|          |                                                    |
| :------: | :------------------------------------------------: |
| 打开文件 | with open("filename",encoding='utf-8') as csvfile: |
| csv读取  |        import csv<br />csv.reader(csvfile)         |
|          |                                                    |

字符串 "the number of trees : {0}"**.format**(n)
