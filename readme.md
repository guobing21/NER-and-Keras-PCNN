1 BiLSTM 依靠神经网络超强的非线性拟合能力，在训练时将数据变换到高维度的非线性空间中去，从而学习出一个模型。虽然 BiLSTM 的精度非常的高，但是在预测时，会出现一些明显的错误，如实体词尾后一帧依然预测为实体词尾等。

2 而在 CRF 中，因为特征函数的存在，限定了标签之间的关系。因此，将 CRF 接到 BiLSTM 上，就可以将两者的特点结合，取长补短，通过 BiLSTM 提取高效的特征，让 CRF 的学习更加有效。

3 通过 BiLstm-CRF 模型，结合简单的数据集实现了整个命名实体识别任务中的数据处理、训练与预测。 

--by liuguobing