# 数据可视化大作业二

## 项目概览

### 项目主题

大数据可视化

### 小组成员

沈溢鼎、吴元昊、陈佩佩



## 数据

* 数据内容：

  ​	葡萄牙波尔图 2013.7.1 ~ 2014.6.30，为期一年时间段内出租车营运数据

* 数据大小：

  ​	2.03 G
  
  

## 文件组织结构

项目文件已上传至[GitHub](https://github.com/Yuumi0221/BigDataVisualization)。由于GitHub上传不了大文件，因此除了原数据以外的csv文件统统没有上传。

```
- Sources
	- taxi
		- train.csv
- Code
	- HeatMap
		- dataProcess
			- getStartPoint.ipynb
			- statistic_hour.ipynb
		- total (内含csv大文件，运行代码可生成)
			- TimeData (csv大文件，运行代码可生成)
			- index.html
		- hour_1 (内含csv大文件，运行代码可生成)
			- index.html
		- hour_2 (内含csv大文件，运行代码可生成)
			- index.html
	- RouteLine
		- routeLine.ipynb
		- routeLine.html
		- routeLine_files
	- TotalAnalysis
		- TotalAnalysis.ipynb
		- TotalAnalysis.html
		- newSource (csv大文件，运行代码可生成)
- html
	- DVPPT
	- HeatMap
	- Road
- images
	- DVPPT
	- HeatMap
	- Road
- PPT
	- DVPPT.md
	- DVPPT1.md
	- DVPPT2.md
- ReadMe.md
```

### Sources

原数据文件所在文件夹

- **taxi**

  - train.csv

    原数据csv文件

### PPT

此次项目PPT由网页端进行展示，PPT传送门：[「数据可视化pre PPT」](https://yuumi0221.github.io/slides/DVPPT.html)

* **PPT**

  三个PPT源文件
  
* **html**

  可视化后导出的html文件，用于展示可视化效果

* **images**

  可视化后导出的png图像文件，用于展示可视化效果


### Code

此文件夹中中为项目源代码，由 JavaScript 和 python 两部分组成

- **HeatMap**

  - **dataProcess**

    此文件夹中为 python 文件，进行数据抽取与预处理

    - **getStartPoint.ipynb**

      抽取起始坐标

    - **statistic_hour.ipynb**
    
      按小时颗粒度进行时间段分片

  以下三个文件夹中为JavaScript文件，进行热力图绘制源代码，因涉及到本地文件读取，请在localhost中打开

  - **total**

     整体热力图绘制

  - **hour_1**

     按小时颗粒度分片后热力图绘制，0~23时按顺序进行时序动画绘制

  - **hour_2**

     按小时颗粒度分片后热力图绘制，添加交互功能，可选择查看制定时间段热力图

* **RouteLine**

  - **routeLine.ipynb**

     python文件，进行数据预处理、数据清洗、路线清洗合并、路线绘制

  - **routLine.html**

     routeLine.ipynb的网页预览文件

* **TotalAnalysis**

  - **TotalAnalysis.ipynb**

     python文件，进行数据预处理、综合分析、图表绘制

  - **TotalAnalysis.html**

     TotalAnalysis.ipynb的网页预览文件
     
  - **newSource**
  
     经运算处理后的数据文件
