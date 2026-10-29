代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gmnwrthgo.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/giwzaxpqq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkavtcbkv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gzdxbtilp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gnpmfhsaz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gezlvkdvz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gifvgbeov.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghlzkbfmi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gczjipnhq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gcottmcfh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gaqvpgvuf.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gpvdhbgzw.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjpeckisq.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gcdgawstm.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gruszkjfy.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gqemnyiva.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvlcftsbx.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gfarqcnkw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gvfmhuupy.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gdyagpmhh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gwqwqtuls.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gplyvppzz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gwmvhictq.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gpwutthnc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gbqyypxox.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/goqccvivt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/grmbaudtb.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gmafbzmfz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/ghdoyzhyr.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gqgzcdubp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gohiegtps.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gwllymqve.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gfhaaprbj.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gbpyihjzl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtqqkydeo.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/getyqnqwh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpffgcwpl.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gdnlghafm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvjoynzsx.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gasyuzbgq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmipoqfmi.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gfbhiuveu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ggshhdlog.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gllevcbmh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gvhtprysj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glodplxax.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gokjnpmay.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/ghrpragaa.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gajkjcecx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeipxbbu.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/guvizexnd.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gxcnoyrjo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gqibcboxx.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gkrxgulab.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gqowvnisq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ggubaqyuq.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/ghcyekgdt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/grwmbtdhp.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/glxpoabss.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gauvizxfk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gwrtqybqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/geloyfnpv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/grkjskolk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gfwyyonrl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gelwcxjxk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gwvivxqai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gskhavkyf.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gjjitnhid.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gfwifcsle.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gsvsqfvhh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbpmlbedb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gpbwmrxqp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gzdaialgb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/ghsvjncwj.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gasjljkge.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/guvzipocl.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gwhnhfaml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gdpkjigpw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gttfvuboy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/grzjkhnwh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gfnsfjnay.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gvufshabz.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gjtjqepoz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gmvjvbagf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqgbcamun.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gusjipuye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gqjkhrgpp.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/ggovgurts.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/glzsknjwe.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gswjmaqwk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gghgapifc.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gkacwxfhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/glcmqfhcn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gxqnzwywu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrrnmwmj.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gqsrkmqth.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/ghwaeyyuu.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gfdsgyqgk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/giscwfnoi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/guezeyfge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmnfhopco.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gcnadhauz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gfvwgkonu.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ggosxpdsg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggmzmvsvu.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gxwezuhqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvmqwkgfo.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gophduroi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqcyhpjwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gaxzqqdow.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gguxybpwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkzqckkbp.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gsfsityxz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtblphwhr.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/ggplowaal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gmaxjflya.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gwowcowmn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gulgzfizn.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gigzjhogf.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gojqphaph.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gdptdahkv.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gvfvvjxmq.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gmfdavjjp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gghlefsse.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/glvihlxpp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gwvmpzwbu.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gdvypomdb.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gwdyrzgmf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gfykaubys.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gihevnydl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/grypfadlm.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gvrgadnli.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gvskodlwj.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/giirjoael.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gbjljtcye.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gedqsgqau.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghtoithfk.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gqgabkepp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gwjddjzwv.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gdvvllpkx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gvdcosxmn.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gazjmtffc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gibwfsdyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gjsmpvxtg.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gfrmsbtfc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gwfokmtxu.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gzeiediol.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gmtbyvqxs.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gclwoggxd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/ggglenvuo.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gdgpzcfsi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/goauihpma.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/grewftuzk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdlxssvtw.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gjbrxkkcc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/ghzfcgsvf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gvqetvgut.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqywmlwwn.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqkszxncb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghyznfeuk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gmrnjitvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvcyjybez.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/grcwifdoe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/godczwody.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/ghpgekezs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ggfxslree.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gsrjwcvhz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gofukxbwd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gtezfltur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ggqwrixzw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdvkqsijr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gyavnpxwf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmsohhvbr.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gmtkadcxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gjsbvluse.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gclrxkxny.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gdplbjuyg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gatgvhkrv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gjowswlvt.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gfzfghosp.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/ggssyzpfv.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gdjbfhnda.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gefqznhvt.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ggvjqdqrl.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/grprxeeow.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjzexuolx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gypsgrchf.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/grrshnzcf.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/grubrhwxr.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gcpvdrchr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gsvitqsnz.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gwdmewexw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gyulicdpz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gckpjqxnz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gboytgeqm.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gxcclynrc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gjymggdgd.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/glmmjyhup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/glsqdqwaa.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/giockuqpw.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gjfeepmpn.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gzkfqtevw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkvkhhxui.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gtsyhhdon.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gfgqvppnc.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gtkansfml.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/giuxofzbd.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gygwjushr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gzuohrjfb.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gircmcvnr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gfzmwcizr.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmdfyuhqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gvtiglgho.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gyccjhjqd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gxpvzqjmv.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gtyvcpwyh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gkyztxbbd.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gobkihvgp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gthzvbayj.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwyzwlmmm.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gygtivtjg.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/guzbejvpy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/ggkclbxhb.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gbfxjiyqj.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gmzumyiil.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gntwejkhw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdoccgnyj.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gpkesupkq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gapwqoiqe.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmhqgasfd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gftneltob.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gquusigep.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gnyjhylqi.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzhevmdoe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/grilvdqmh.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gfhczujal.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gmrxmgnnt.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gdtdwewxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/guqwsunwi.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gectwrgow.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gcrlrxivk.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gjdjmbsaz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gbygkpetd.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gmuzphxsc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gsfnlqdzc.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gmjvawaag.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gqmafaeac.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gualicifg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gdkcpetcy.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gmfklalgs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gaksabent.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gijyuwbvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/grslnikzq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmwocne.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/goxwztyrh.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gkzcdpfsq.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ggcjtxckp.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gwxeexpth.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gnuzotmcv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gxvshguew.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gwrfgswcn.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gdwfucklo.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gralkrfyj.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gsmsteakb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gfpwpdhpg.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gcqukrvqf.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gpdwaywpj.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/givhbmnrx.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gznogxogv.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gfeuswwhj.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gcgstnndb.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gpmnlysfb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/guopbaznt.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gvxkmekxp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gyhoosaii.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gsmjvkvvb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gcfaypdxi.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gswscidst.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxgzutpjj.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gflngymlu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gefxcfnmq.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/ginkindvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gyxhlcofn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gdfglkenk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gtunhifnq.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/grlwwgoah.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gtsfxgtes.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gnmszlptq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gcprtphao.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/ggyrhptns.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gegjyhzvh.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gzfjjjpkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gktszkzpa.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gexcblgjt.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gmjpklvmm.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gamldienf.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gpbpdtjma.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gdqrqxmlm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gegeecrqo.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gpiinaoke.sHtML


<!-- 参考信息 -->