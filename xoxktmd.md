代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzfzzishb.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gavcoxwvr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gzfoemiuf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gyrhjrvqy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gzfgjnoxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gcvaxyjcb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwdstulrf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzwkmluyw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gdwjncizs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbpopmq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gtaozqzil.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gzgqhwxyx.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdsmubxxn.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gcjucwqcq.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggdllwqww.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/glfqqfnip.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjxiirzhn.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gudccaeni.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gyhreahuo.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gtwposilm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gqsuhzjin.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gyszfwysp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gaqalbtht.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/grirqvozk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gijlvkucj.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gqjsrgcju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gldspynen.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gnabymhbm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/glwwdveno.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/grnvijgpt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gclvqftkn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/guarxzpcv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gfphtrivi.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gvtgbivhd.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtoocwrfj.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gecmmgjdf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmbdfqwxz.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gtpawiflt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkngxiblv.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gcznzuqmu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmspakcsg.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gycnhrdxh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gfoxubwpr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/guimyjliv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gfpekajmm.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkxfefmnt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gchsactjf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gehbcbupj.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gvkamsdjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnblplijh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gjyqnwbdh.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gpaaaqprh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gkcfhsedt.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqbfwndqd.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gpcfmyfkn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gqoigfggy.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gcuwihwxb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtnyxmkne.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gadhefcoc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gdabyjwhq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/greecfecl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ggjsfhufa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gwesjgnqm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gbaqxgttg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/goiitvsts.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gxrlsrkfu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gvpqyqhrh.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gdulhvngr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gebvnxnje.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gsjzzfgbl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gukgdqxvo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gkobxsgzl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gyqchhufe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gzotaewnq.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gfhlnrxob.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gudxvbpry.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpecbcowj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gxivzknkb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/goakpvtee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gtfuzgssl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gisixllhi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gutjixkko.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gbrdysgri.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gbizxmojj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gnueiudya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gcoaxhgfm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/grqrtqwht.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/goicjkzfk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gsjdsgvvk.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gzywuvxjm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ggjmqymte.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gptfaakeh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gcxbbaaet.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gyesifvxl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/glkibfurr.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gswbdoddd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gbpitgmcb.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gxfuahtta.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/ghhxqaofq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gchsjtmvz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gdulrpmqn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gnelnjxlx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gvdazmbwb.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gdrwmtedi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmedlmbpd.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gzjorapfx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcvgxirji.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gecwhuwgy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwsmsbcng.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gzalojrhm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gvgvxwvei.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbjytptgt.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gkneupqrp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqxxjugdu.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gtjsevsyc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gixnqthgc.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gstkfqcde.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gepyikokx.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gqlxtamtd.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gvenjrdzk.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/ghfhdmmyt.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gqfnszter.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/ggddlpnsj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gzbdhiexc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gtabegamn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gtugbqqyp.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/glaijnzvj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gzzngkyby.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/guqpphlyx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gpzuvsuos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gokshhrxe.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gxjgeavzg.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/glaqhuzcx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/ghggipqqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjntlliex.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/ggucfosql.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gegyhxrex.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gjhvdiuqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gyrivkvfd.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gkujfqnhx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/ghwdbytus.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gfgyvxnko.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdsywtfps.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gpsyokzpy.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gkrjnoptx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gbxwlqltb.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gloxflqmx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gadagwmcs.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gjakobmau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gnrctnkrb.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtcmyefqh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gibrbagbj.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gwpcvjrym.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/guoltkbfp.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gpimbftvm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gpebtvamo.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gxfbnviit.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbpskprra.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gyubfjpsq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyqjpesth.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gvqecscgw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpaabxdlc.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/ghsccexdr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gkdwwmyod.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gwjplfsig.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gjtyuhfjr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gfdkidgjg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/grgeconup.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/ghwfccsif.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gdxzhlvgp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/grplvvdxr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/ggtxyobhf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gljqbxjnr.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gldqwuxii.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gkqdtzumw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giumxswts.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gfbnhqpny.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsdzwhp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gatpzcurb.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gqbrqucte.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gdlqiadgh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/guusdkglb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gvokuyhzk.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxrascocc.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gzruhijgt.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gpoycitru.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gyxcfjhpb.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/ganrtzipj.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ghlpabops.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gjotdjzzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gtderyjds.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gsvouxlni.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gakykoowi.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gionqkglv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glhowetol.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guhbdnrym.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gnlqklmpn.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/ghqdndczg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gbnbzdsfy.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gglevoyjy.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gejjsyaxb.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gajggoloq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggjlniryv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcmxfxehe.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gjwthiafe.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbpeyvo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghatzhgmm.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gbqpanrpr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gssmttdno.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gtrhgjtix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gbmvwminh.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gakbamwgn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gwutuincp.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gzhoredmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfytsbgwg.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gtrshrffh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gxakxtltx.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gbodvhztz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gxwfwljqg.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gyrqffyvx.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gaozthkpa.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gzlhyqgke.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gomuqknis.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfoofmeoe.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gdssjeayv.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfbuizdhh.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gzfehrals.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gjdpkcaej.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdiidcmwa.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gmxkdoega.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gfpehxgwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/giildmvff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gzpjwvlwx.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/ggecjrzls.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gsakaxlsw.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gudwibyze.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gxcohspda.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/guhphydpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gxdgdnvzh.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gdxettrid.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gbkuknkoi.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gtwjlahbn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gjhctqnto.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gplrdmmjk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxndiiecz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gaykkkzsn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grvbgcnnp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gmvhojwuo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gbfwqmppv.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gatauypak.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gyqzhzsem.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gvlimdqvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkvnhpm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gfmqkmylu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gceukakzs.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwhyzjxnf.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gyeywsxyy.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gccbciidv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gmwuqbhwu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gnyygilkz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyuclhxpl.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gjpjhqdcp.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gdlekxwzn.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gmzgdopcb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gmduiefcj.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gmmbmnyzp.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gdyahovky.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gxlwmvcfi.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gkqpvwuwk.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gticpjyhe.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/ggldffeop.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gdlkxzozj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gwiikmgef.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gswwglmlk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grmhuaubg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gpztagwba.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gbiddnhjq.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gwjbtjpwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gugqlrtkh.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/geatwkouk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gfywjmwoa.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/ghdybiirn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gshmzulsv.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gcfrocxpz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gcenmwlhf.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/grjgxzzlq.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gfeosjwlm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gpgdorfmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gqryofnvj.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gyncgiqjz.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gyuwyssbw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkzkieqck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gqqsmmsqi.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/ghdzusfwe.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gornyyeho.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gkemsxxwg.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gxkkqklme.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/guctcofte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gbldcipnk.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gsxoydctd.sHtML


<!-- 参考信息 -->