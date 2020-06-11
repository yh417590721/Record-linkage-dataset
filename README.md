# Record-linkage-dataset
课程项目

数据集简介：


        数据集包含记录与来自记录链接设置的个人数据按元素比较。
        任务是根据比较模式确定基础记录是否属于一个人。
        这些记录代表个人数据，包括姓、名、性别、出生日期和邮政编码，这些数据是在几年的过程中通过迭代插入收集的。
        这个数据集中的比较模式基于100,000条记录的样本。数据对被划分为“匹配”或“不匹配”。
        因此，“is_match”是结果变量。注意，“id_1”和“id_2”不应该用于预测，但可以用于根据找到的匹配构造连接的组件。
        
Attribute Information:

        1. id_1: internal identifier of first record.
        2. id_2: internal identifier of second record.
        3. cmp_fname_c1: agreement of first name, first component
        4. cmp_fname_c2: agreement of first name, second component
        5. cmp_lname_c1: agreement of family name, first component
        6. cmp_lname_c2: agreement of family name, second component
        7. cmp_sex: agreement sex
        8. cmp_bd: agreement of date of birth, day component
        9. cmp_bm: agreement of date of birth, month component
        10. cmp_by: agreement of date of birth, year component
        11. cmp_plz: agreement of postal code
        12. is_match: matching status (TRUE for matches, FALSE for non-matches)


任务简介：


        该项目将实现一个端到端数据挖掘项目来分析所提供的数据集。其目标是实现一个工作流来预测数据的目标变量(即分类或回归)。这个工作流必须包括两个阶段，如图1所示。
        Stage1:数据探索
        这个阶段包括在Python中使用Spark的DataFrame和RDD api来研究数据。
        通过查询数据的一些重要统计度量来理解数据集。可视化数据并解释你的发现。展示出对所分析数据的深入理解是很重要的。(注意。在这个阶段你不能使用熊猫和scikiti - learning。)
        Stage2:预测分析
        这一阶段包括三个机器学习(ML)过程。每个过程必须包含至少三种ML模型(如决策树、随机森林、朴素贝叶斯、前馈网络等)。这些模型必须使用通用的度量标准(例如准确度、精确度、召回率和ROC)进行评估。
                过程一的具体要求:
                 •在此过程中所有的ML模型和评估方法必须从
                在Python中。除了ML库之外，您可以使用任何Python模块。
                过程二的具体要求:
                 •这个过程是用Spark的ML库构建的。（即pyspark.ml和pyspark.mllib)
                过程三的具体要求:
                 •这个过程是由TensorFlow和Keras构建的。
        
  

