1.select \*from player where level>=3

2.select \*from player where level>=2 and level<=5

select \*from player where between **level>=2 and level<=5**

**between用错了WHERE level BETWEEN 2 AND 5;**

3.select \*from player where name **gaxy** '^王'

**正则关键字写错了REGEXP** 

4.from level,count(\*) from player

**GROUP BY level;**

5\.**from** level,count(\*) from player

**应该是select**

group by level

having count(\*)>=2

**6.from level,count(\*) from player**

**order by count(\*) desc**



**SELECT level, COUNT(\*)**

**FROM player**

**GROUP BY level**

**HAVING COUNT(\*) >= 2**

**ORDER BY COUNT(\*) DESC;**

**排序是人数就count 是等级就level**

where **exp**>=5

8.group by level

having count(\*)>=2

**9.order by count(\*) asc**



**SELECT level, COUNT(\*)**

**FROM player**

**WHERE exp >= 5**

**GROUP BY level**

**HAVING COUNT(\*) >= 2**

**ORDER BY level ASC;**

10错 select后面只能加聚合函数或者等一下要分组的列明

11\.

对

12select level,count(\*) from player where **exp>=2 and exp<=5**

group by level

having count(\*)>=2

**order by count(\*) desc**



































### 正则查询规则

**4️⃣ 正则查询（REGEXP）**

**name REGEXP '^王.$'**



**常用符号：**



**. 任意字符**



**^ 开头**



**$ 结尾**



**\[A-Z] 范围**



**| 或**









## **LIKE（%或者\_放在哪都是有顺序的**



**%：任意多个字符**



**\_：任意一个字符**



**name LIKE '王%'**

**name LIKE '%王%'**

**name LIKE '王\_'**









**写法1：统计所有 exp 值分别有多少人**

**SELECT exp, COUNT(\*)**

**FROM player**

**GROUP BY exp;**



**写法2：只统计某一个 exp 的人数**

**SELECT COUNT(\*)**

**FROM player**

**WHERE exp = 20;**









