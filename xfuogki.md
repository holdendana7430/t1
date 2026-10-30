代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gcxglsbca.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gughdifdi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gwambowkx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcawhotnb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqndafuzk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gewcoebab.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjfteyqi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/glpjbspym.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgprtjue.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gmravfcdg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgzvfclx.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqfuzzod.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdthxwtn.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/goypaxhaa.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuxkiftd.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/ghlhfryco.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbpdfmng.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxzacbfa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkllzjmoz.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpbslew.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojoymhkk.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtapulizw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhpzgjsu.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkgmpxdrm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtvedfua.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbneikvi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/goxngkyga.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfcwfkwd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzgfbjjk.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gfevqoiou.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkjjizfxu.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwqkfvtf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrrkovol.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/giewrhqmp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glixdpzfu.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxlzzkws.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxncbzmep.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gobjwzeeq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geijlyhbm.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/glkurttye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrjihki.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwupytf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklrcujhq.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmgctdc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glbbulzzy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gecngidik.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnefahry.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gnlnhfzew.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaeaxbjf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgttocrb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdevwwdv.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gampprqvp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/giuhhtcug.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzukayifg.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteidokgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gogsjgaek.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvazcdvxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvmwafhm.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpdrrport.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpvqbmcz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/glramtfvu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhsvfoal.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsdarwbp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/glgkzgemp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/grkewqjhb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gatraugsu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/guvmhstqe.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvjxdhvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gsldpkvlx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtbiwjzt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzceyvzu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpmdghky.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gffaomqky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkllbbogy.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbbryply.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/glukmwffp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnebycond.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauituzu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gbtnruduk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuefgqeo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxunwyqe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimuirnsa.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/guurzaafw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbozjtwis.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpayzytsj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gzxwntbfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gvixubpgc.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gbzxvwnbx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdxvulwo.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/glikuyixh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbcteyhf.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gzifdrlgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkerifyo.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/grpwmgcce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvzhqpow.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gsqrzgfwh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/glsremzvj.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/ghccvnsvt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gfedkfvee.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpinloaec.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gnaphuzkw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gniqwnyfy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghupfxime.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/giuynghlc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvpuukw.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbdpszrt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwbtqcw.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajybozdy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqlpnacv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhieccxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gmamtxvfp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvrxbqvq.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefsiobil.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqffsfhs.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkcnmzmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/grigxiftr.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvxwwztr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginqrlsbc.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsiszowhs.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqshlupca.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgveyzbu.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdtksuze.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaokfawl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxlmpkqc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuseudgr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsukcmti.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gxoocngmh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhyjjcfo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugthjtwq.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxpwtaqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddemdjjn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gestcbfwq.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjcidnw.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gnmoaqzhk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gqmewrdpr.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gtzpleqrw.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnjocjomt.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gmnfwvlus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzrqffw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqvkzwvk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfyajlib.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbxwskt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcmnffxiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gbxgzehfp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grovgwemr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwayyzcs.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ggqrmdgva.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflyavxsz.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggctlshrj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzykkwecs.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxfyndgg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gszgpcnho.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfznymde.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gooovxjlo.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giztxsnsx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuhoivls.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtuiomhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goaqoaunk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrzkxnms.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gacibewzc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvyvxiws.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdaqlxkv.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gllbunlde.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgvvpaer.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlcsofqs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjcdcrgc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneetrnej.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gskrefcld.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgiskwdv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfprfcxsy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grwwlgaeu.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbxtsgqeu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtcbyucb.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpemjtra.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjgwazgl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/girllunsn.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gifhbxkvk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvxxarhw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzklskova.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gnazpxgxp.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnbhwxem.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtymmqix.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gaoqcorwk.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnijxhvz.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/guszodmpb.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdgikhcvv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjtmyya.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnlwddjr.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gflwxxoxu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdxepbbu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjosfiykd.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grlkpgnov.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gskaawluu.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzinfyaqv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhhqdpxv.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/giftooanu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsxbszzhe.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjdogixog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwqcndxdc.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gasfomoot.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwzmpoji.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnxvtmryq.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glfeeinnd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhjacpee.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gaoyxqadd.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcrbkfajo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcknrtqgj.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyymnjfu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gexjhbpql.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbkqunlq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqsvzvx.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghghevlza.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/getblxzbi.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpamwoeuh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/garpxxmcw.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gghopajwu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/givkwjnii.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbijlaijr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviyubkko.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjgfqvgb.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzdhidg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnlivkup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdrnmdjj.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gaccvsqzx.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaknomqiw.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbdmzltc.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtofgpapz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gauzjiidz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhpcehxy.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtpynnusd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnspdlvku.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxrirfgn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwbildzt.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukuebqzh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/glhladhhh.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gtntnefqi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gughiwpsf.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatjouiwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gzgezutip.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlpmopvs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grcgbrfif.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnixlmoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtqgbhnw.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbsoydgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganjukzvz.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdsqkmxqg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicpqzegr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gsosofavw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblukayj.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gwfcqngod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/glrwbkyaq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghfgrhmc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoomwypu.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjtupnodd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvfwbqgfa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtatijjln.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcytceeg.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ggmxnaylk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmcyatyg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gonmorchg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfcidhxr.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbqixsca.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfegpqjl.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggnodvywj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpiskkjlu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwxthiaf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbnactv.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxckqemlc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyfnlbxa.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqwiptgo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnsncyxr.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvbxltyy.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ggyfvumft.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemrvgbe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvbnmaew.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/golnochsb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuaqiqqq.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbwacsh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzlrjes.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsdpfnmo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gyunuiqkb.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/glnkvsgrs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gekmywbli.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwisaqtd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzppyqgkv.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmttuevi.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmzzxyaaf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdmctpcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gddxpdtzh.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyyrgmivt.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlalqkei.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gdygexepp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gdvwazutu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvjjalwf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqmkmge.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnzjatcl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcuwvnpb.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpczipwci.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/grehylckv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhqicdob.sHtML


<!-- 参考信息 -->