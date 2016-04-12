
Open Source大黑客你好:<br>
>我下午把modify.cpp里面的各种数组看懂了，在准备建模的时候遇到困难，再请教你一下以下问题：

- [这是我的建模示意图](https://raw.githubusercontent.com/lucyking/pic/master/IMG_20160413_015719.jpg)
- 建模的时候是先将图的数据读取到二位数组里 然后遍历数组将特征更新到像modify.cpp的各个特征数组中，然后```solver1.loadProblem(matrix,colLower,colUpper,objective,
			 rowLower,rowUpper)```加载问题，cbc中有没有更加高级直观的保存变量系数矩阵的方法吗？
			 
- 我觉得保证某node只经过一次或不经过的方法是：∑(i,node)-∑(node,j)=0；  但是这个表达式写起来复杂 有其他更好的方法？ 是否能提供一个和modify一样直观的cpp样例？

- [modify.cpp l:69](https://github.com/lucyking/Cbc/blob/master/Cbc/examples/modify.cpp#L69) 这里用到了一个函数```solver1.setObjCoeff(0,-100.0)```
这个函数是设置什么偏移量吗？ 我去搜过是否有cbc API手册不过没搜到。网站上这方面的资料似乎比glpk少，你可以提供参考手册之类的文档？

- 感谢你在论坛的耐心解答 期待你的答复 ; )
