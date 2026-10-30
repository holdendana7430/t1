代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gyirupwpe.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gqjvhizpy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gspjdhfmd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gzscsmalk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gvxpkmjdm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gojwvpoar.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gcsehmjre.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/geqbsohmp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/grlpiqafh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gihjbsygi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gzqohpcwz.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpzjqpuyo.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzbxyexzz.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gacxosieu.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggawmhtvd.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/grsjtuhjm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/glwaeawxi.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gqkbkybnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gfippfdmd.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gkeismoey.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gzrlplhvh.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gyjnggnun.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gowahzkvd.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gpwdmqznh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gwlipznjk.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/glxrusgvq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gzxeikjjd.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/ghgbjqsod.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/givoektmy.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gqttuzllr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gpfansslv.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gbpjwsqlp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gqbjmaiqn.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gatnbgmqe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghmuegcel.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/guuaslqwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnzrkarjb.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/ghfyysfmi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkchnklky.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gzsnrqfbv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkayqjtam.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gnuplcwlq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/guqovgsxr.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/getdkgibp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gtnxuxnym.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfwqxbwmr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gzwwlhedv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gnmhicvto.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gsxxfzczq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gwebpfsax.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gyotoiokl.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gsxnruyyh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grjebnnbv.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/ghywghqsq.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/glmnzumny.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gggyavvbz.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gjnpzsgxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbdhyioao.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdghnjsme.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gefkxswam.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gffvtezvj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gobluvavp.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gwctvetjp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghgzsirxo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gvhdhqqju.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gziywqtaf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gxojrcxez.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gjlmjdjxj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gvnstrbdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gqjowtwxn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gozlogqqr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gzjeaseys.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gzyhqmmpk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/grjfaoxub.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gzxwpbjuh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gbxtntkwh.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gojptbffs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gopjxapaq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gtxtocysv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gsijvlixa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gradyhgmb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gztwjcshi.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gyxrppobk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gkpedvlmt.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gspyxinsh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gajyibqxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/grtumjfhi.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gkepdqcej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmfgqprvm.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/ggqkzypca.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gvnreoutq.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gocaeodxb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhrdowv.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gykztlivz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ggquodvev.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gtcknzwso.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkehhdsjc.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gpzxzrokr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gmcownwol.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gjmusslap.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gnyyjtoyi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gbublolgj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gojarljux.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gcjyzvqth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gafmjtquo.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/glxvbtetq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjlcvvalu.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gdbquxhhw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxjzgjxws.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gwbzkswyq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/giqlmsxzu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gcfpyeeth.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/glvvamonz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvkweuavg.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/galagigvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxinfkpeu.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gcjeatyby.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gttxfergu.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/grkqygfbe.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gvcuhfqmf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gphhwyfrz.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzfkyvko.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrxpchl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gxwrleosc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/giibgixyb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gawopahsh.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/ggeepjwne.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gjzjzggce.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gbfqnkqly.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gnoublrcr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/googewvmo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/ghxvljdtu.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gsxzuxtvp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gjjcveoxl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gektoghhr.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdhgogr.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/glecgjanb.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gzcyxmodq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gvfdcmohm.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gpltdmiho.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gobezluar.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gucfftrjx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbbyspqad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gdltomlfd.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gqcwofnnw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gmvavpthk.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gdvtsksxy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghasauoqt.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gjzjtfaoq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gxskukdoa.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/glkjfoslz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/guuzilfbs.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gqoboegwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxojiqzot.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gindzddcb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfiwznkig.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gexegvvfo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbfurpecf.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggmbaswhw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnubmxgkc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/giwjhzbph.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gadfpucdc.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gtuzwtddy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gnldsxxpj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gkjnszrpo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gyjttjfrw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gbzsqtsrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gwnirinsd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gbjwtlxep.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gyhykyvhv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gmhpfshgn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gtufccxfg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpqidsi.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/godceqxss.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmtbhcg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtwkkqzfn.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gdeccsgdc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gisgffpkt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gbxwdciyh.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gvnjbpiqz.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gomavprco.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gpbmgljyn.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gqcclkbxe.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gxxudpqpy.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gdrajxwmd.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/ggqpddvbh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gqhovqszt.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gqyjxzihv.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/garyscwfk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gxrnoetas.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gofxvgvsn.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gsqwqckbe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/grdrrxgbf.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/ghqsylpow.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gonrvhnfw.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmkgcbipj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/guxktbhct.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gtjgdaoaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gduqllpen.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdzkfclbz.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gioaenelz.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gtzzihrvo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/ggtxinkfq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gevszydpn.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gyofshree.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gnljwwvhz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gvqdijdzi.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gcahipfil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gppiapaak.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gzirulwgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gpckzlpoe.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gkrxdjrmr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gkjkfcqqt.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/geofruqkj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gsuhpwzqe.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gdaonbnbg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gtxqfyiot.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gnrxctpem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gtxnolwwt.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gowpgqlxa.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gdkrdddgn.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/grgykorwt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gqdwlifsb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/grhtvnudg.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gxcdpqvbj.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gvbamofzs.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gmebfqryd.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gbfgxipei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/grzmjmskd.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grrguqrpf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gnioemhjl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/glveyxmbi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gkwvrkpvb.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gsiztidgp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gppbubhsp.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/ghybawhkb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gbkxbgskb.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gtmrbgkng.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gicvxlkun.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gkgfunknj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gcsvzexky.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfoealj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gucospqga.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gaxtapbuh.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gjinzjebe.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gamrepbbt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gmlkpxywp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/grfpdhbah.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gpttxolhn.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/giajadrdq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/ghzzfepki.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/grcqjectk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpvokac.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gvxmkhzcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ghcvshspw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gqzobyxsx.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjfockfsp.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gocyleady.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gnzwpmsqe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtaxosk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghugpokre.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gcxuptjhr.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gwnuducuj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gyltobtdc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gsqkbyqwa.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/ggzhntihd.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gdonvagel.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gwfzqxuph.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gptupdjoq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gpxxqoxpm.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gdklyqkrc.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gojbxvumv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/glbpiovdh.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gbmfftjez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gdnmzezxq.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gvafszcvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gduppbfai.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gxieqhvgb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxjarkhyl.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/grakmptld.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gxlwkoyrk.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/ghklrxvmj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfsaxuptn.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gzvkdrqxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gqdcdjvre.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gbjilqveo.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gqdojlamt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gkjowvtms.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/grkfwnnad.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gmolxfrbm.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gvmjuijpn.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvqnkvzri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/ghjfunvml.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gkkligdbj.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gydsbuify.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gmyxttgjw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gbdjcjtpt.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gnlcrbamm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gfriuumnv.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/girqfdpiw.sHtML


<!-- 参考信息 -->