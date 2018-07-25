# louplus-ml-
实验楼 《楼+ 机器学习实战》 每周整理 &amp; 扩展阅读 


## Week1 ： 
### 常问FAQ：
1、有关于LinearRegresssion 中model.fit() 函数详细介绍[文档](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)

2、modeel = LinearRegression  和 model = LienarRegression() 有什么不同？
			Link:....
      
3、[ 线性回归] : 中为什么要用， x.reshape(len(x),1), y)

**重点代码：**
      model.fit(x.reshape(len(x),1), y) # 训练, reshape 操作把数据处理成 fit 能接受的形状
		
    1、思考以下错误出现的原因？
				"ValueError: Expected 2D array, got 1D array instead:
				array=[ 56  72  69  88 102  86  76  79  94  74].
				Reshape your data either using array.reshape(-1, 1) 
				if your data has a single feature or array.reshape(1, -1) if it contains a single sample.
				"
2、为什么需要 x.reshape(len(x), 1)
			
 思考题：（对于上面的实验上下文），以下哪行代码能运行？
 
					1、model.predict([[150]]) 
					2、model.predict(150)
					3、model.predict([150])
					
### 知识点整理
* 最小二乘法
* 回归


	

**最小二乘法** ：
 - 1、[最小二乘法本质](https://www.zhihu.com/question/37031188/answer/411760828)

- 2、[论文：最小二乘法的历史回顾](https://wenku.baidu.com/view/17b16411dd88d0d233d46ada.html)

- 3、[函数逼近中的最小二乘法](https://wenku.baidu.com/view/9bb1553143323968011c924d.html)

		  
		  
**推导公式需要回顾的知识**

		1、[多元微积分知识点总结](https://wenku.baidu.com/view/e06572607e21af45b307a82f.html?from=search)
			重点在于， 链式法则， 以及求二元函数求极值问题
