# bank-complaints-classification-based-in-BERT
Main work:
•	对数据进行清洗，包括去除HTML、URL、emoji，以及处理重复文本和无效标注数据。运用欠采样、数据增强等方法改善数据类别不平衡的影响。
•	分别采用全量参数微调和LoRA微调技术对BERT模型在数据集上进行微调，并通过精确度，召回率，F1 score评估模型的分类效果。利用LoRA的方法，在仅使用全量参数微调75%的时间内，达到了全量微调97%的效果。
•	采用balanced cross entropy和focal loss对损失函数进行优化，将难分类样本的召回率提高4%。
•	搭建了一个自动化的投诉文本归类pipeline，为银行客户投诉处理提供了高效解决方案。
