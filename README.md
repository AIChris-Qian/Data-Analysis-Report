# 数据分析报告

**概况:**
------------------------------
针对某款游戏的数据源进行数据分析。

内容要点分为5个部分，包括: `每日活跃用户` / `留存率` / `VIP付费率` / `不同等级用户组成` / `不同等级用户付费率`。

使用`SQL`作为**数据提取工具**，使用`Excel`作为**数据可视化工具**。

**数据源:**
------------------------------

某款游戏

时间为2016年11月21日—12月20日
      
    新增日期：用户创建游戏角色的日期
    活跃日期：用户登录游戏，玩游戏的日期
    游戏天数：用户截至活跃日期，在游戏内累计登录并玩游戏的天数
    首日等级：用户第一天玩游戏最终达到的等级
    首日VIP： 用户第一天玩游戏最终达到的VIP等级（付费金额越高，VIP等级越高）


**数据处理:**
------------------------------

数据源存储在`Excel`中。首先把数据源转换成`CSV`格式，然后导入`SQL`中进行数据分析。


**分析部分:**
------------------------------

内容要点分成5个部分，包括：
     
     日活跃用户（DAU）
     留存率
     VIP付费率
     不同等级用户组成
     不同等级用户付费率
    

### 1. 日活跃用户（DAU）:

   绘制两张可视化图，包括：`日活跃用户组成`以及`用户活跃度`。
   
    日活跃用户 = 日新增用户 + 日留存用户
    用户活跃度 = 日活跃用户数量 / 月活跃用户数量


### 2. 留存率:  

   绘制留存率可视化图，包括：`日新增用户`以及`次日/3日/7日/14日/29日留存率`。
   
    N日留存率 = 新增日之后的第N天还登录的用户数 / 第一天新增的总用户数

    
### 3. VIP付费率:

   绘制三张可视化图，包括`日新增`，`次日留存`以及`7日留存付费率`。
     
    VIP等级分成三部分，包括VIP1，VIP2以及其余VIP。
    由于VIP等级与付费金额成正相关，因此VIP等级代表了付费能力。

    
### 4. 不同等级用户组成:

   绘制三张可视化图，包括`日新增`，`日新增`以及`日留存用户等级组成`。
   
    用户游戏等级分为三个层次：1-10级，11-20级，21-30级。
   
   
### 5. 不同等级用户付费率:

   绘制三张可视化图，包括`日新增`，`日新增`以及`日留存用户付费率`。
   
    用户游戏等级分为三个层次：1-10级，11-20级，21-30级。
   

**补充说明:**
------------------------------

关于**数据源**，请参考`某游戏数据源`。

    / Data-Analysis-Report / 某游戏数据源.xlsx

关于**如何使用SQL处理数据**，请参考`使用SQL`。

    / Data-Analysis-Report / 使用SQL.pdf
    
关于**数据处理代码**以及**可视化图表**，请参考`SQL代码`和`Excel表格`。

    / Data-Analysis-Report / SQL代码
    / Data-Analysis-Report / Excel表格
    
关于**数据分析汇总**，请参考`数据分析报告`。
   
    / Data-Analysis-Report / 数据分析报告.ppt
