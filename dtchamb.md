代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gehyogxur.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gwawcttae.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gkmlkycoi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfioqxmjx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gkyzgusoq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gvenqaxtc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/glbxqlijl.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gjyzqhxaw.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsfsnjclj.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gzuyarxsl.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/giodxcpfe.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/ghhkslprc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gksysshcf.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gnlipnqjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gvvczzvln.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfwzftkse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gkrtvohoo.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqrvshhtw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grmlfdvnu.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ghowayiso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gecblntmn.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/grgeyytwd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/goircbvio.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfyjtdb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gddghzrbz.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gszzonqzr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gswnwuceg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gyxbemsaf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/ggzxbusmc.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gvbwrtemq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqorhslny.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/glddudzkq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gawljxdpt.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gcmaobaxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpgfcwyip.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/grnqrwqvo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsbrdqjdq.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gygbroien.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gsknzjuuo.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcrizlowl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/ggbecrhsl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/giliclzol.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/getdqmiuq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gmbraqhmf.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gvsgaoxmx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gkjshobse.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gqiailecz.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/glchcloze.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gbulwitgg.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfbbhcizy.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gttofdrwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gfhijeodb.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gjyqnhfyq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxxvhbzfe.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gfhafemdo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/ggqosjgom.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gseumheib.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/grzznidqj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gxexehjbi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gbzhufjly.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gkdnkjyit.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnublrtzv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gopztpscv.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gitwmoqve.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gzyvnheta.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gsqbgrgad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/ggjrdyqbw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gexjovdgy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gterkwkop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gnuhhtluo.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gpxdpwjzh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gtopadywz.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gujiiobro.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gztzhnycj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gurwarjku.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gccsyfoue.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gclnigquj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ghlyxwjdu.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gkndjlzdk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gqzwpsuuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gqfqqrioq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gtkmcicqr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/guraqgddz.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpowamnop.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvdbjubnn.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/geecigwjt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqsudephr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gcbzjxjmq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gocuajcgf.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gmpdrkvmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/griwxiiie.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gsztjvgdq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gfbnjrkdc.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gwjlookiy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/guyppvlza.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gdpvsofyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gcyugnhmj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gfmvmhfmq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gvsqqrbry.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/godecbtgd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcadfmljk.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gluxwhxfr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsuhjjoso.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gmwjehwxf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsritmrkc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gnsvvqzyb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gbatovlms.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghcpxztwr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gcznisovw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzpjbcqng.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gxuzslnbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gpwdbzbgi.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/goxlayxig.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/grfyhfire.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gzodoqgif.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gkbnzzwvi.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gqzjuuaeu.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gtebqlnjr.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gnmtyaotz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gxpqbffoz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gkprhrged.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gbedlhsqm.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gtomsjufw.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gdbhnsqdw.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gdrcgnavm.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gugidlhhe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gqduufitg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gotwhdfwt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gmltenfzq.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gixrlnzlb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gxrcxhhso.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/guftfxwtd.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gquupyuxm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gmcsfujzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gzdioutij.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gpzcqntew.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/grwjdjjxp.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggplcoeau.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/grvtmndyn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gmoaxdgpe.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/giqcayqpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/glzdnyvvu.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gnwwngjyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/glnrpeqzi.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gygqlzman.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gdxxhqwzs.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/girwazobb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gcbzjrskr.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gbgtivvzw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glpgihgyi.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/grgqnnoxx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gkwityiiw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gpabzzvqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giezrazdd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gulixacrn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnxsbnvvp.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/grupzjahy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gcjhsvgmp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/ggqaxaeja.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/guxlkttgg.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gsfivkndm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ggcjuyfgy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gowsnrrsf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gbulvfadw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gbvcijglu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gmkbuzguz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvutcchwn.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/geqxnwsqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gzvdabvib.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gwieahpyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gktypkesv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvlzbnonj.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/goegzczhw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gesrwevag.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gzkcuxucs.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gvifuldcz.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gvolnxrss.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gazhisscs.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/ghtziogqc.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gmltkmdwh.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gexjqwnch.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gztwtcnpo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/grfupetnj.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/getkkwepk.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gkavxelqz.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gtvnrevkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ghzqjstus.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gshloumik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/ggtqsngxt.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gpuinwueg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkikyihme.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gzklpryhb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gbnjokosf.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gkhdegkdl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gxmdghhca.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/glsgwkhpg.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gtciqplzj.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggevaztnv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gzurwmaoy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gksunzckk.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gztyzgiit.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/guwogbepu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gyowxxexg.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwynvrgdi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gxrgwibpx.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/globureqv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gujhnobuh.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gheslaczj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/glohedrmv.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/ghapjzzpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gutjtfudb.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gftvwwtxa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gkovskvkg.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ggwdyhqso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gnyyinigx.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gpkyevtdw.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gapipoyqq.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gkjadklrj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gtvimscab.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/guhfrdivo.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/godzdtzno.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gyqihkjhv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gcxsdcrlh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gghpyupse.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gqgzjmhpn.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gklzyypsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gndxrccsb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gwijducdb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gycrdoddq.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gxbvccolq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gyeapgcug.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/geibvwodr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/glnpttgaw.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gfendbczz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/ghcnobkqj.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gmwuaggdy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/guheyitvg.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/giwilxumj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/ghevisgji.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gwsaqgxuc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/glktbzffi.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gviqyijdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/garpmzvpx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gyeyluiyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gquwktucq.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gajbzwbci.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfnsdpqfl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gdxkbxffk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gxsxihccf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gaskyoiyz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gvohwjzhq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gnncatfea.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ggnnjeury.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gzalsuivj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gnqaoryap.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gbaxwedfz.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gtysoecja.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gdmtgwdeh.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/grojwgegu.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gohjwhghr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gmfkljbcx.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gmccbmvyz.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtxcbcqjr.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gzfdssdpn.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gkrteyqpd.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gcdktzhxv.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gamlmtbhj.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/glatqrwui.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gphyyzloc.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gayjumtdg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gtwximlto.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gcnylmcrd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gzvwfcsec.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gwawoywbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gbhsrbslo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gsdqqkzqa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gnscwxhen.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gqsesqxdv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvtecxfpz.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gvpexhzgz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ggtwebduy.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gvakkjzgm.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gzbdhjymw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ggltiqhjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gmfprljas.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gxyupaujv.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gyaamzscz.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gnclwrweo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ggclfinsp.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gnhgxcpuf.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gwnapsrbv.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gayiwypaw.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gkehrrmqn.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gfguylkzl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gxflnqpyj.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gfbuftfoz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gkpvjyuoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ghimbyfjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gknikhpfa.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gjpzteige.sHtML


<!-- 参考信息 -->