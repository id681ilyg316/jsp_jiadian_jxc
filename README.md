## 本项目实现的最终作用是基于JSP家电进货销售库存管理系统
## 分为1个角色
### 第1个角色为管理员角色，实现了如下功能：
 - 供应商信息管理
 - 员工信息管理
 - 客户信息管理
 - 库存信息管理
 - 管理员登录
 - 系统信息管理
 - 进货信息管理
 - 销售信息管理
## 数据库设计如下：
# 数据库设计文档

**数据库名：** jiadian_jxc

**文档版本：** 


| 表名                  | 说明       |
| :---: | :---: |
| [t_admin](#t_admin) | 管理员表 |
| [t_client](#t_client) |  |
| [t_provider](#t_provider) |  |
| [t_repertory](#t_repertory) |  |
| [t_sell](#t_sell) |  |
| [t_staff](#t_staff) |  |
| [t_stock](#t_stock) |  |

**表名：** <a id="t_admin">t_admin</a>

**说明：** 管理员表

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | adminId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | adminName |   varchar   | 255 |   0    |    N     |  N   |       | 管理员名称  |
|  3   | password |   varchar   | 70 |   0    |    N     |  N   |   ''    |   |

**表名：** <a id="t_client">t_client</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | clientId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | clientName |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | clientPhone |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  4   | clientAddress |   varchar   | 255 |   0    |    N     |  N   |       |   |

**表名：** <a id="t_provider">t_provider</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | providerId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | providerNo |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | providerAddress |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  4   | providerlegal |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  5   | providerPhone |   varchar   | 255 |   0    |    N     |  N   |       |   |

**表名：** <a id="t_repertory">t_repertory</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | repertoryId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | repertoryName |   varchar   | 255 |   0    |    N     |  N   |   ''    |   |
|  3   | repertoryQuantity |   varchar   | 255 |   0    |    N     |  N   |   ''    |   |

**表名：** <a id="t_sell">t_sell</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | sellId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | sellName |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | pn |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  4   | cn |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  5   | type |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  6   | count |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  7   | price |   varchar   | 255 |   0    |    N     |  N   |       | 价格  |
|  8   | saleman |   varchar   | 255 |   0    |    N     |  N   |       |   |

**表名：** <a id="t_staff">t_staff</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | staffId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | staffName |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | staffPhone |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  4   | staffAddress |   varchar   | 255 |   0    |    N     |  N   |       |   |

**表名：** <a id="t_stock">t_stock</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | stockId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | stockName |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | type |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  4   | count |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  5   | pn |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  6   | price |   varchar   | 255 |   0    |    N     |  N   |       | 价格  |
|  7   | date |   varchar   | 255 |   0    |    N     |  N   |       | 日期  |
|  8   | saleman |   varchar   | 255 |   0    |    N     |  N   |       |   |

**运行不出来可以微信 javape 我的公众号：源码码头**
