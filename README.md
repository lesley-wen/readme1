# readme1
Naive Bayes Classifier on MNIST Dataset
项目简介
本项目使用 Python 实现了基于 MNIST 数据集的朴素贝叶斯分类器。MNIST 数据集是一个包含手写数字图像的经典数据集，广泛用于机器学习和计算机视觉领域的入门实验。本项目通过 Scikit-learn 和自定义实现的方式，展示了如何使用朴素贝叶斯算法对图像数据进行分类。
文件结构
代码文件：notebook.ipynb（包含完整的代码实现和实验过程）
数据集：MNIST 数据集（通过 TensorFlow 的 Keras API 加载）
依赖环境
本项目需要以下依赖环境：
Python 3.7 或更高版本
TensorFlow 2.x（用于加载 MNIST 数据集）
Scikit-learn（用于实现朴素贝叶斯分类器）
NumPy（用于数据处理）
安装依赖：
bash复制
pip install numpy tensorflow scikit-learn
运行代码
确保已安装上述依赖。
打开 Jupyter Notebook 或 JupyterLab。
加载 notebook.ipynb 文件并运行代码单元。
代码说明
数据预处理
MNIST 数据集中的图像被展平为一维向量（28x28 -> 784）。
像素值被归一化到 [0, 1] 范围。
在某些实验中，像素值被离散化为 16 个整数值（0-15）。
朴素贝叶斯分类器
使用 Scikit-learn 提供的 GaussianNB、BernoulliNB 和 MultinomialNB 分类器。
自定义实现了一个多项式朴素贝叶斯分类器（NaiveBayesMultinomial），用于处理离散化后的像素值。
实验结果
通过 Scikit-learn 和自定义实现的分类器对 MNIST 数据集进行分类。
计算并输出分类准确率和分类报告。
实验结果示例
以下是实验中可能的输出结果：
plaintext复制
GaussianNB Accuracy: 0.8345
BernoulliNB Accuracy: 0.8123
MultinomialNB Accuracy: 0.8567
Custom NaiveBayesMultinomial Accuracy: 0.8456
注意事项
TensorFlow 的安装可能需要根据您的系统环境选择合适的版本。
如果运行自定义实现的分类器时出现错误，请检查代码中数组维度的匹配情况。
实验结果可能因随机因素和数据集划分而略有不同。
