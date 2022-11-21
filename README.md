# 使用dataflow将外部数据加载到dataverse中

## 实验一 在 Powerapps中创建dataflow

### 1.1 登录Powerapps，在左栏Dataverse下选择"Dataflows"创建dataflow

![image](https://user-images.githubusercontent.com/34478391/203108488-48ed10a4-c536-4090-92e8-7515766f5be2.png)
### 1.2 命名dataflow，如果创建standard dataflow，不用勾选 "Analytical entities only" (连接到 Azure Data Lake Storage的时候需要创建 analytical dataflow)

补充：standard dataflow 和 analytical dataflow的区别： https://learn.microsoft.com/zh-cn/power-query/dataflows/understanding-differences-between-analytical-standard-dataflows

![image](https://user-images.githubusercontent.com/34478391/203109869-db255872-6e0c-42c0-858d-a23a7db85ca2.png)

选择 excel online中的数据进行读取

![image](https://user-images.githubusercontent.com/34478391/203111052-feb64066-4a6e-4aea-adfb-32a50cc5e913.png)

![image](https://user-images.githubusercontent.com/34478391/203111143-d3236495-ba78-439e-b9e9-52bb1b7398fd.png)

![image](https://user-images.githubusercontent.com/34478391/203111218-762fa5c1-75d4-41f1-b3f7-222d57baec25.png)

