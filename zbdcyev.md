代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gmwofqgnz.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gdpbqqvvm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gixjoxhmg.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gctmcihes.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/grojppfvi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gpkthimjf.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gkeukxoxt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gtcvifwjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gplajnpnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gcgzkalqm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gorqyrnsg.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gwkwhkqgk.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gycdmseyp.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gyykftasa.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggkvqdizo.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gyzpuxfrg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gjnmwguet.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gzwcnaquo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/glwvomklc.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gzqpdnnsb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gstnqprbl.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/goseutstd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnweqlqwl.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gmhyfqzms.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gnfalgsnx.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gvonbxlia.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gtsrwhncw.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/geboagiao.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gysrcqgmk.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcfzckxcx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzzqwwadc.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/giomanvzy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gzwhpcglr.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gdpgrkfqg.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzhpsfmyw.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/guvdbgibv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gbkdukray.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gljvnqzng.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdmkdsgjn.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gawinfcat.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/girhihtji.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbybdxcpo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gzddsakpj.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gohepjgei.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gtprnicmi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/guzdxompb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjzwtwvcs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/grfgalzda.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gswzvmgmt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gsbvdxlhw.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gymxpzdvq.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gpzqptkeo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gvnjgezyp.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyvctrpig.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gosmofzej.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grxnwxxab.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gzymesbev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gkkvabgby.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gjdaiicjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gntvjrrge.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gjnlrehvm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gizmzefgc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gooqqkeyl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gdbpofgtn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gvziqcmpv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gwcosfylw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/giktpeglx.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gkcncixtg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gucdkiehn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/geripldlv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gntkvhgfz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gpsejedcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gwetjicim.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/givqhlcjf.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gkponooos.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gwaoiepwq.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gryyjsaid.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gfxakgnnt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gxabffagv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gwjsngeau.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gjtsjmjbd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gceiaylzi.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gvwidgdwl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gfytbmfgo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gufckkvwf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gxffunvuk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gjlwldnpc.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gtmpquzur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gepbbnkoc.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gvbiadzrh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gndoocuba.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gookfjfpn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gatuefjpr.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gkbpapxku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxkfsrtsl.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gedokftma.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gsdlbbswf.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/glypohtdm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gswlladuu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gxtapmbse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/grkdfkbux.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gohoosaxk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gagygmcix.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gcmlpoono.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grrzovyjn.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gemrbrwxj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqsosilgq.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gfxsffzyj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gunzjtjis.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/giuakpqps.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gekrvzscu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glyeveyvy.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gbzpgpaqz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwdkfwgxf.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gkvrhkwab.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqavagkmq.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gstulpiou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/ghwgnqxzx.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gsermnxgp.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gqwvukhuq.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gswcbilvr.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/ggopqeecz.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gctydzhkj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gmvnzgdbj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gtdncbmhv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gpchucpmq.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gdxhfjhjy.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gymxcxzpb.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ghqeqnstt.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gbowktqqj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gavjjqvtm.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gwytfdxnx.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gfbcnqxlj.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gvdmvdzig.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gvqnbknro.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzgkfnqug.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcobnmsml.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gdnwgggch.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gyvuauslc.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gfkwlrgdp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gaetyuefx.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gyntecoah.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gyomgyeme.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gktblqwpt.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gehpdotrz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gcascircd.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gjigdgffh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/ghfpdmide.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gqzvduzwz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ggyvzyxmy.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gauojcfmr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkqtzhsvz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/guzpcdxmr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcaacdupx.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gzctgiawe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxvxbyski.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gfawanzyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmdjmwahz.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxqgyglrl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gklyobccf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gzphzpwtm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghirehvln.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gbfvxioog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gnxzfkums.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/galcvzbbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gpkxwxwdf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gammedqml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gxtoptrmc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gjvbwxwdl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gjhdvavrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geoqifwjf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggvfoltue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gmsphdxrb.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gewehhwke.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gbnxocdcz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaueoblwl.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/ggmfkhfuz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzlmzztle.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gbiesotwr.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/glglnakve.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gezmxuedr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gxlatfdwo.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/geelzwbfw.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/geegwjvnj.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gmphqsbte.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ggvwgrmho.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gyfngrzel.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gqucmiszx.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gotskwosr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gddozsuzp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ghryokssk.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gjkfanovd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/guyrtqbgx.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gpkeopbnw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gfxhoppdc.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/givqkxuaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gdfhrexys.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gxxsbkgfx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gdnaizlon.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gzbfqgofi.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gugvubmum.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gysfrpasj.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/guwyawzfy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gymzsackn.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gufijeupj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gswmjjqwm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gnscnownf.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/grmnjmmti.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gexaicgus.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/giazlbyca.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gxgbwnmcv.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzcfzxvzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gykfdfxvn.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gcgljamgu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gnpwiiyyn.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gpalcdral.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gcruyshvs.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gsyuzptqj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gmdkbcmyh.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gcpwyurur.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gecgzqbwh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggahfghnd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gsjejpubf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/ghgzvqnlk.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/giggykzer.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ghrndmgja.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gjcswwdqk.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gcwautpbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/geerxpvnq.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/geurwxueg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/grhouchov.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gtcngtxmz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gheyzvyte.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/ggtfkovam.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/glrmagrut.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/goedlnony.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ggeuawbns.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gterkfhgm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gdiksgdug.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/ggwyzzynt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/ghwenvanb.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gybxzzztq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gevqbigbg.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjbdvkudg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghjmyqnza.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gialtvdlg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gebtlddqm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/ggyjjhscv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gbwadgymz.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/ghozkkxtr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gtkrecudq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvdsagcyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ggbsyeegb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gybqegbaj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gjmzzhcxf.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gsnsbmqik.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ghuiqeozl.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gnjornkxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gmxzogfoo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gkyenznvj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gwyngvxpr.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gfljdxegr.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/ggmoetabl.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gpwvgogvi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gofdsgczl.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gkpmzuoka.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqttqirlo.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gghhmaotv.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gvjqubetq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/guveiveyr.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gcdtpjxge.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/ggiocolfe.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gbtmkszvs.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/geyljsqkh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/giormfvmx.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/glcocegkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/geeriticm.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwmzizfqh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gzhtzynbi.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/glwxgveim.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gmrzzvego.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gfmkfkjhf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gworktlvl.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gkegpylod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjanbwtlj.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gozhzuzzn.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gdvzocbov.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gslmucwgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ghngbyhtw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gesdgcerv.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvoukldol.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gorxjsmky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gauynqzgx.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/geuuebuga.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gmzvowqhc.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvkpewajg.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gaqmszyvd.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gizvhhvbs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gnyhowalg.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/glxhepjyw.sHtML


<!-- 参考信息 -->