代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxutntzm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/getguqqov.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmqrqpco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gguglfjli.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpniadhl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/goheyhzcb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrtnbqfq.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gdexshflb.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goisxnyed.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gjngloxda.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gihrzvujn.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwombey.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjkqbgqu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/grfkeneju.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfythmkvr.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gmhsmfuwq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpbvozl.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmpovjcg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsltlddc.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmvsbvud.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/glnqeztdx.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/godqvbyfc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gryrerpph.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gtyqxerim.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gccztsuwe.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gjfljnrry.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geobhabru.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gydlrqool.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/geryqtmaz.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/goommksxh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpzwhaev.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlrjjqys.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmyvupops.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfsmtpwe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzboqoppk.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gihhunmeg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glkjdinwv.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/ginpsvskx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfoboofv.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhwpqrb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvbhgmeh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqrqqoxdi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadvbxgqi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/grldzystx.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gpbsrakvn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeuyejpx.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gcihxysfz.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotpixiuf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gytbypvmw.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkttprw.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/glvjejpqe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnsdudssn.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gvhtkrjkl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggevemrml.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdyxcghjr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwpdgwll.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gkjidsxhq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gclnkjwte.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gszeragnr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhqenyd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gzejkcalr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gigxbgiyy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdntsqfs.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfzethnqv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxewcrg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gpktqzoye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/grngytawc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxnadfycj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gmqqljfir.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbodhkvs.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviahwaik.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gimirsrut.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graetybyt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlgwlpbp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmepklt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbcntuot.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggikdwzqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/getnmcsqn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhucfyrh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/glaouemkq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqniiswq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvpwbwru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtiqbosx.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gzifusavy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzrcozva.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtuvwqij.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gmkszqzbr.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghtjzyanh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtgfmso.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gcapudvjs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/goaogsyos.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizuhxwo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gqykgsvmd.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghubnxrdj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gitdrefth.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuxqgnea.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsfgzcob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gnjswzfat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/geikmrdwe.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gdywxuigi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbenznr.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gfnxogkof.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdnjfvxb.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacqxncso.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgqextr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpofrxte.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/ghufxckpp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoskuoyx.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmfqoqr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/givimxauc.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gidtjqppn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzsvybgv.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/glmiczict.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gmsnfsbol.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzobventg.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gxcffietb.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmkooeez.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcijxngxm.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gulceqqhb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gohosdvah.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwskimk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdhsqpxh.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsyjeltk.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyospxmse.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjdvovws.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/ghneeiubq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gyvnmaklh.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gojeaufxx.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gszslwrnl.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gukagibvq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gietgfxqh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoqqleck.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gevinrumc.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gcxtujvyr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkzebwek.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gnyizcfxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeyhrsoc.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gthaobvxe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzeimkbh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrvhjqgk.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacrfmlbp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdliqnts.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtineztn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gtnydbxca.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gmhcqneem.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gffkgjxzc.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjvwmnc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gyxzthwlb.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/geesadhvv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtzpokmg.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrxplork.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulmkoync.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoeecqvj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqijepml.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwcindoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geizkkbth.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gzonwvvih.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtznabgb.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwazayoma.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzibsew.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/glwsxjfru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgsyvyab.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/guctumnva.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdgslxve.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gutfbkgoe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfcsrnhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbznfxka.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhtzfhid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkqyjwsv.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgzlhuvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqujkhkm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjybjvph.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuowuspc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glvuirisj.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gasdiojtg.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gydpwltmg.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwdkuohp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gugnkxrix.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpifwniix.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gryuuhmlt.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gkwmwtutu.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnowzgxg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzqatyyt.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnijren.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gegjrmcip.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gurugfetd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvqormtt.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczcabsmg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gairrqowf.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gurdyoizv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxhunaka.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavxvjso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gladoyyac.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjuctzl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanrtqjv.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuepqffx.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfsuyksw.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrmfwjft.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gulrodpgy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxblnoaeo.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghzhxcup.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduytmilv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwtuawrt.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gencvdjtt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggwtiefzp.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gstakjjfh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdjnkjywh.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grlfhvjrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvbokbww.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdlyfscjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfgzqfpoo.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gcoebdgoh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glojruzwe.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqasdgfdw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwufvnnu.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghkdiwawm.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqdnoup.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkviqialt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glbkycfgz.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/grhafdkzb.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggzhcglbh.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfcrcfnr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjahihglv.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggnrrjjcq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnziriwdy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/guvuyndlo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkerdzh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gvvsebylc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyioauzwc.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gviwunqks.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvformjo.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/grhpudzts.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmgvpnxs.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gbthfievt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/goufytayx.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzjivdb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxljxcov.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgvyyczg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzuflslp.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqveawgft.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glrvhjwyr.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghtzmapft.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqazpuzsr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqmpdui.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggatatwwe.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gggzuushr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxgyrua.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxttejfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gxcvspffq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggraypujj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gigdrupzp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gguvotfnt.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjlqeojm.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/goqazfhlj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gurfrpmow.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gomaoxezg.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gsxdqbhxj.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljehrwup.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeupbbhz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzdpvedu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gyhsqodsy.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/geccyqfsp.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqxmhnvuw.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/guntzvtkc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/giopegdne.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/goosvpkbb.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdqgkumtc.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjlluwemy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztjijkie.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhafehiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gafroueit.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhcdunxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbrpbdmqd.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gqiazjhfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqkpzbhrw.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghlaaicut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmctcyvf.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycvaigss.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggjusmieg.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gubpuyaqz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsdvrmbi.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gevohqsqz.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggkppfmmj.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gnozxmudt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatpicebw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyguavkw.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gponydhoo.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexjoodt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfpmvcor.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gshexhpul.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gwynybrvh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtioatiep.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqegyju.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijhvqgtm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gybthqhtu.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbfamqmm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdtdklys.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gscnklizf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/guekhimaq.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfgduttd.sHtML


<!-- 参考信息 -->