# 使用dataflow将外部数据加载到dataverse中

## 实验一 在 Powerapps中创建dataflow

### 1.1 登录Powerapps，在左栏Dataverse下选择"Dataflows"创建dataflow

![image](https://user-images.githubusercontent.com/34478391/203108488-48ed10a4-c536-4090-92e8-7515766f5be2.png)
### 1.2 创建并命名 standard dataflow

如果创建standard dataflow，不用勾选 "Analytical entities only" (连接到 Azure Data Lake Storage的时候需要创建 analytical dataflow)

补充：standard dataflow 和 analytical dataflow的区别： https://learn.microsoft.com/zh-cn/power-query/dataflows/understanding-differences-between-analytical-standard-dataflows

![image](https://user-images.githubusercontent.com/34478391/203109869-db255872-6e0c-42c0-858d-a23a7db85ca2.png)

选择 excel online中的数据进行读取：

![image](https://user-images.githubusercontent.com/34478391/203111052-feb64066-4a6e-4aea-adfb-32a50cc5e913.png)

![image](https://user-images.githubusercontent.com/34478391/203111143-d3236495-ba78-439e-b9e9-52bb1b7398fd.png)

![image](https://user-images.githubusercontent.com/34478391/203111218-762fa5c1-75d4-41f1-b3f7-222d57baec25.png)

![1669049035462](https://user-images.githubusercontent.com/34478391/203111940-da85748e-c71c-4426-992e-1bea2f005730.jpg)

选择excel文件中的table "Devices" 和 "Manufacturers"：

![image](https://user-images.githubusercontent.com/34478391/203112381-824f3bcf-1c1a-4066-a191-4b658707adbd.png)

![image](https://user-images.githubusercontent.com/34478391/203112805-3b7b283c-7c90-440a-aafc-02fbae95670a.png)

在dataverse中重新创建 Devices table，同时选择"Device Name"作为UPN：

![image](https://user-images.githubusercontent.com/34478391/203114387-a237fc2a-3782-493c-93f4-248bffefaa28.png)

在dataverse中重新创建 Manufactures table，同时选择"Title"作为UPN：

![image](https://user-images.githubusercontent.com/34478391/203114531-19249510-667d-4942-9b68-400e9b1265df.png)

![image](https://user-images.githubusercontent.com/34478391/203114620-95f65161-4371-49c2-8c71-9565c46fbf30.png)

### 1.3 创建成功以后，可以在Dataflow 和 Dataverse 下进行查看

创建成功以后，可以在 Dataflow 下看到 "published"状态

![image](https://user-images.githubusercontent.com/34478391/203115458-1cbbbe27-96a4-4646-b5c3-210dc427629e.png)

创建成功以后，可以在 Dataverse 下看到创建的 table

![image](https://user-images.githubusercontent.com/34478391/203116360-d267066f-0a0f-4253-9559-a68b74d24dd5.png)

## 实验二 在 solution 中引用 dataflow



