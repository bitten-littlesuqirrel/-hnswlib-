# -hnswlib-

这是最近研究的一个小demo。主要完成用户提问，匹配问答库中的问题，返回答案。

首先，把问答库中的数据提取出来，送到bert中处理，然后储存在hnsw创建的向量空间中。

然后把提问者的问题送到bert中处理，得到句向量。

再与hnsw空间中的向量进行匹配，返回匹配到距离最近的一个节点，返回该节点的标记。

通过该标记直接输出txt文本中的答案。


bert处理是通过调用huggingface提供的接口。

本代码只是项目最初期的自己写的一个小demo，有条件有机会的话，在更新一下新版本代码。
