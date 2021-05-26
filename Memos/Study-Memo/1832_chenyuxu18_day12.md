## Day12



### 期权 进阶篇

课前回顾 

1 基本的名词术语和解释 

1了解期权的基本策略和组合策略

 本次课涉及到的各种名词术语

典型的四大策略 

 买入/卖出 认购/认沽期权

基本策略1 买入看涨期权

​                 优势 方向做反 损失有限

​                 杠杆效应 

​              劣势：时间价值不断衰减，波动率下降 对买方不利

​                  买入看跌期权

​                 优势 损失有限，杠杆效应，以小博大

​                         资金占用少，不需要保证金

​                劣势同上

​              卖出看涨期权：损益图翻转：赚取时间价值和波动率下降的利润

​              优势 ： 先赚取权利金，赚取确定的时间价值 卖虚值期权容错性好

​              劣势  收益有限，损失无下限

​       期权策略组合原理举例：买入认购期权，卖出认购期权 （行权价和价格不同）

​    牛市价差 适用场景： 短期看涨，不会无限上涨，短期可能有波动

​                  买入一份行权价较低的认购期权，卖出一份到期日相同，行权价格较高的认购期权

​       熊市价差 

​                  买入一份行权价较高的认沽期权（平值，轻度实值），卖出一份到期日相同，行权价格较低的认沽期权

波动率上升；

获利模式：

高杠杆博方向

赚取时间价值

盘中损益图的解读

到期损益图叠加时间价值的曲线



  波动率交易

  典型的组合策略

2 希腊字母

对B-S模型中的期权价格公式进行泰勒展开并且忽略高阶项

delta，gamma等

delta 期权价格随标的价格的变化幅度

gamma :delta的变化幅度

波动率对期权价格的影响



3 买方和卖方的风险控制（期权）

   买方：

​    亏损原因： 方向猜错了

​                        方向猜对了，波动率/时间价值衰减快/合约选择不好

  风险控制

​    卖方：

​    胜率高，防范低概率事件

​    遇到小概率黑天鹅事件，赔率暴增

   期权策略：

1 对行情有一个观点

 2 用策略表达观点

 期现结合 备兑开仓 ；保险策略： 保护性买入入股期权策略：

买跨：预期波动性上升：预期大事件

卖跨：预期波动率下降





推荐书目

3小时快学期权

波动率交易

python金融大数据



蒙特卡洛模拟

一类基于概率的方法

随机数的生成 numpy.random npr

均匀分布 正态分布 泊松分布等

应用举例 计算圆周率

期权定价BSM公式
$$
S_T=S_0exp((r-\sigma^2/2)T+\sigma\sqrt{T}z)
$$
模拟BSM：

直接模拟

变换后取对数，模拟

离散化求解（几何布朗运动）
$$
dS_t=rS_tdt+\sigma S_tdZ_t
$$
Zt=标准布朗运动

应用：期权估值

欧式：使用几何布朗运动对指数的变化进行模拟



 

​         