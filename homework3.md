### 作业（10月17日中午前提交） ### 

1. 用不同的可视化工具呈现同一个数据集
  
  * 调研目前免费的可视化图表工具（国内外都得有，在线离线、交互静态都行）<br></br>
  * 在 Kaggle 选择一个公开数据集（可以只截取部分数据）<br></br>
  * 用你调研的图表工具（不少于3种）呈现上面选取的数据<br></br>
  * 在 markdown 里列出所选数据集、使用的工具及呈现，并附上使用体会<br></br>
2. 之前提交不规范，或还没掌握 markdown 基础的同学，修改已提交作业的 markdown 文档<br></br>
3. 按个人需求和计划，消化本周所列的链接内容，并注册公开课学习
<br></br>
### 选取数据集 ###
* [World Happiness Report 2019](https://www.kaggle.com/PromptCloudHQ/world-happiness-report-2019/kernels)	
* Data Source : http://worldhappiness.report/ed/2019/Context <br></br>
* [下载](https://github.com/G-York/Newbee2/blob/master/world-happiness-report-2019.csv)
<br></br>


#### Introduction ####
> The World Happiness Report is a landmark survey of the state of global happiness that ranks 156 countries by how happy their citizens perceive themselves to be. This year’s World Happiness Report focuses on happiness and the community: how happiness has evolved over the past dozen years, with a focus on the technologies, social norms, conflicts and government policies that have driven those changes.
#### Columns ####
* **Country (region)** &nbsp; Name of the country.
* **Ladder** &nbsp; Cantril Ladder is a measure of life satisfaction.
* **SD of Ladder** &nbsp; Standard deviation of the ladder.
* **Positive affect** &nbsp; Measure of positive emotion.
* **Negative affect** &nbsp; Measure of negative emotion.
<br></br>

### 选用工具 ###
* Tableau
* Hanabi
* Python-matplotlib
<br></br>
### 数据呈现 ###
#### 全球幸福指数排名（with Tableau） #### 
![image1](https://github.com/G-York/Newbee2/blob/master/%E5%85%A8%E7%90%83%E5%B9%B8%E7%A6%8F%E6%8C%87%E6%95%B0%E6%8E%92%E5%90%8D.png)
<br></br>
#### 幸福指数与人均GDP和预期寿命的关系（with Hanabi） #### 
![image2](https://github.com/G-York/Newbee2/blob/master/%E5%B9%B8%E7%A6%8F%E6%8C%87%E6%95%B0%E4%B8%8E%E4%BA%BA%E5%9D%87GDP%E5%92%8C%E9%A2%84%E6%9C%9F%E5%AF%BF%E5%91%BD%E7%9A%84%E5%85%B3%E7%B3%BB.png)
<br></br>
#### 各指标相关系数矩阵（with matplotlib） #### 
![image3](https://github.com/G-York/Newbee2/blob/master/Overall%20Correlation%20Matrix.png)
<br></br>
### 使用体会 ###
* 上手难度：matplotlib > Tableau > Hanabi
* 自由度：matplotlib > Tableau > Hanabi
<br></br>
Hanabi的操作界面最直观，出图也最快捷，但是操作的自由度较少，比较适合对较简单的数据进行快速出图（在网页上操作也更容易卡顿和出现bug）;
<br></br>
Tableau是我现在最喜欢使用的可视化软件，但本地化不如Hanabi，直出图不够符合我的审美习惯，需要在ai里再加工;
<br></br>
Matplotlib说实话我不会用，但是kaggle上有许多Kernals，我找了几篇案例大概copy了一个代码。

