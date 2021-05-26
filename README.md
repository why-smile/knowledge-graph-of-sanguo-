# 基于百科数据的三国时期历史人物知识图谱的构建
## 项目内容  
本项目从百度百科中通过python爬虫工具从[“三国”](https://baike.baidu.com/item/%E4%B8%89%E5%9B%BD/5428)首先爬取了数百个三国时期的人物，然后再通过每个人物的关系栏补充与该人物主体有关系的同属于三国时期的人物，最后对所有人物的百科网址进行数据清理和规范化处理，同时，为了查询的需要，另通过人物实体信息框中的著作信息创建多个著作实体，最后提取所有的实体信息框中属性值三元组，特别地，对人物实体，提取实体集合内地关系人物三元组。最后将所得到的多个三元组转换为jsonld格式并以图数据库形式存入后用gremlin语句进行查询。
## 项目要求
1. 从百科类网络资源抓取三国人物属性和人物关系，进行数据的清洗、schema的定义、属性的补充以及人物知识图谱的构建。  
要求包含作品实体和人物实体，人物数量>=100，人物属性数量>=5，人物关系的类型>=10。
2. 使用图数据库存储知识图谱，能使用gremlin语句进行基本的知识查询，如“魏国的名将有哪些？”，“《观沧海》的作者是谁？”
