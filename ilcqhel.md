代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyrsatcm.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/ghlrffvgl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbgfgvmx.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdmtnxve.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrobmovf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxccesqlz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkheoodt.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlmbykiq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ghvxbnuvd.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/guckpsrrx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gstizkqgj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/givptnzkw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/glkyfofci.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gfygkzuga.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefekypyx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/giendpllx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqlmpjnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzeumlaq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttifgrdr.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhaizsqw.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/geiacrpac.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gprayumns.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrwtlciy.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gzpinewrd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoufbhe.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grqnqpjkr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gphtscwpn.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotoxkre.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gcujdxgty.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnpjunwa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbxizgsn.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gyquiuuhg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdwtrfmr.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcebrzmb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gdkunczxz.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/geecfliwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtfvnmnn.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gspfhtymt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnsikmcw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcrpblwh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuputshs.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkvqpiulw.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbsvcphb.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxycwzwdn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyflrwgp.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgtbtihp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehjxrser.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzhakszv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmriwtshf.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gqusgwrcb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgzqveoc.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtperahs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gdcpstnde.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxgygsq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrypudnd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcmlkmnz.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gmhdwywez.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gkypwqmqf.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gifdylbly.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gklztbwpe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gmwekhlex.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfcoavnv.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdmvkeuu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjyeolan.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzelftze.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoqaewhg.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gncwijvsw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyfojucd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqotbwohs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhkwzzch.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gruuirkuo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdkkfkk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozhcttxv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gpuddckho.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gyuqsumce.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnuqovvmq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipipbwe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyqmoqbk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypcijbhu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkahewpl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqrhktx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdtxcst.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvixdtrlf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/ghkhqtfmh.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmihmpe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gmawdplue.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gvncomwfa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gquqsfuvp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnbyfvsxt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdihskwbe.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpvmrmxjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqzyenyq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrotitiv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtotjyllz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphrrapwd.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gdozpwqnl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gicuehmfp.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gfrpiivli.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxqrgxq.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gjvchlvbs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkcbqtktg.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvfirsi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkgvnnw.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gisneoenn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gndzyqiei.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnuiimi.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjaxakje.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gdqrvtxui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbudbqpy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkqhljxh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdtlyivd.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumjqbrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbftqfctf.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdksvbxl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glkseiwjq.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gviwojjuw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxcykkle.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghioxskms.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gsynyhxpe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gufiokqdw.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/glnsfhiod.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gasqbyqrb.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjoirehz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxruukojo.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdlydjwu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gacxuqfig.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpwrrtas.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/girjoleyd.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtililgnp.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gksgmxjyy.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyphgnws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbuhgiju.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoillwej.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnlqxrog.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/grufuvgyv.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfezxfwwh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqobuerhh.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqayair.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdonzua.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbqnodx.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwnkidjge.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrgccij.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gtxzpfope.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqtrkrz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoxvcshx.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gmilztnnd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahiovet.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gglrwrypd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqoiarug.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjpfkmrx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giyhdkqlk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeftpnem.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gdalhnfjq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdentgva.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfjtngx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqgixgy.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gillwmseq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggavdqotj.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvunadom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gffbwczhd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclfamfib.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkhjxtjl.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gclkdkmal.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxofzsxt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvpbppyqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqszkdv.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtezscrnw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhhyaqjs.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuiokssb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gchexxsub.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gkhuqzvki.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxvijnvf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/grhzcnuxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gkpeofwdp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmjcavlue.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnytxlhso.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtdavtrr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmqxdpqw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgrzbrnk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxsjxoudw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhimjzqn.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gbazsfxtl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqkpltuy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gewutertr.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlxultfg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzllpchkf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gfcidjzpb.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/glegdnpfr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gzyhcuqdx.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcimhsg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeurtrhz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqpjuwzs.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gapqjwljr.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwnvhfi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaegdymif.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gfpralttt.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gautglwck.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqkecaluw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmjkjjec.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/glitpvhag.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlnohbjo.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqfsrprd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdednqrwm.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkgynwe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdiiqscmz.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjpjdegi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvrdwpcc.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljigppsu.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gqebawzdg.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbaomjymk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqgropv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoakwezy.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/glvnpsmmu.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gujouhnca.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzfwshz.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfglkewz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gequkwmuc.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gregxgzzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gibcfcplq.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gijrfmfvz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goeourifx.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjbpcnls.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlfjdehb.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/guwknqldb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghakrgkin.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gteldauze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gotyrpujh.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlblaiam.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjelxswyk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvipmpy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpixgfw.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glvqvyozi.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gphrzgkxd.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkuktrj.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnnplkkrz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfbnxhnt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/geacynwam.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsbbciqvb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goftrdisn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvdnlmkhx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giltwvrpv.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxoidtfyn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/giepjeouk.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/grwwyxcum.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyrbpqnq.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gogxadilj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gkymwrxoc.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkvcbgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmjjvbfb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsehuwrro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/giuwwwlde.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/grkjeuihr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhsuqza.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gnjceltqc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdwtcoor.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/getyhzqja.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gupqvwybi.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gfjibdnrf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnqxguun.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnplxpgi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ggsugpngc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfntrirt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gumkpektb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gphrbwtpi.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvdjfqwq.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/guexghufx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsahrfme.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/griccoexz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggysprupi.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsljyvh.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoldhwia.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gryzuoyvn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcuzxxvon.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhzyanub.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjqyvlh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieuncufa.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gerqvdyep.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gpequlyig.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gotnnepqy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gkmnrorzo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gufgycrhh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzruwhik.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjmcqam.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gldhfiyws.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcahxkgy.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ggelrlxaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgekczap.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glhfovhfz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjvufqm.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvrlzhvlt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glzxeqvxs.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvitevjn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gffzhlbsj.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gztwkpwyj.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goglqpklk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzmqquhr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmznfzw.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/guvaxlygf.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwnruduj.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/guzugdklb.sHtML


<!-- 参考信息 -->