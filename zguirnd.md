代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/grtgyycka.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gdddewjkj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/grredxdqk.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfflteczb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxiuycsg.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gataoymoe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwojpkfu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstsxulwj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gxbsygqaw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrbsefxj.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gilzjlkdw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvplpnpw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcfpglje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gtduwnukf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gxiksncru.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gjdkdinjo.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpipikyta.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gthyoofub.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gllhfhorm.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gltjebsii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gypueuozp.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glxtxjdjf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbzzjlhv.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwdkfpex.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszyvsaqh.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxhhuziq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyljaklcc.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gcjxvxwdd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gvsdifuum.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/goyfhaszx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibcbvkee.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guargiosq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/glisoxyex.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnreqgp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmwnzajc.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gavsvgeqo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzmzpowt.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqeeklq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goskhmmjt.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhtkeojn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiphlqvz.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gbsntgwxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gultxance.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzibecnq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxklqukje.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gzwcmpzzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxetxqbms.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/grnjcfyji.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnywnzwwy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteqzhini.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gochpfjls.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gjnatgqxn.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gngjqzhpy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gdmehnmzr.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gytypfdzm.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gpvkemuzp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocaxcxq.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpgkdehr.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpveyrspq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxmfykpq.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjgdssbl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/guaqkjycz.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtybchqfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbyfjmnp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gkcvnbbaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswzgzeog.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfyscrgv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwipriif.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gtyxghkhz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkynlgthh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmlsaojd.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/grhbmndol.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gaytdikzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgzgzwle.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyflnvtsl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gttfqhmpc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gamljvsxk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gancbhlmu.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gufbxpqns.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoejnvbt.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmdsndux.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gmcjnwsvd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfhdyevd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gdprrxxlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcbhnutyw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gssgyxbto.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcjfvvavq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxbtcxmj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gilcnppcw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gysflsstc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitexjiq.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gdiczrpas.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwtnalh.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gstivouzo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyhnddqw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdcifndl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbdsrtuy.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/goykickjx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlvvfurk.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gguaqsjcd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqeznpke.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/goekpqoum.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsemalwr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgzymeic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gupjtpsco.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsohcbh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/ggahhfnjs.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/glezasrmq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvhplxmm.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvubsvqbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkexynhqz.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gvmqxgtze.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfifibugu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjolnacgr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkancbjae.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gurcszlmx.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdeuxheh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjyplhkq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gdahcrdak.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gecjyrktg.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsallphe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gocrksmfc.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymzvlyu.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxmtitzf.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnkhkwgh.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtedgcwol.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyehgiolp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gacgyjxoa.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gplyqftzu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanupfir.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gmdnlnlpb.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyijxwi.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcpsufdno.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxhaaiuf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gngolmidk.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/geieexhrd.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gthtnctff.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqyroje.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrdzeude.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjtvyyvdz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxbduchu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoyggcyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gndejoabt.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxncvvst.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gvhqvsssp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvtnhvpa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ginntmxwj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gnndkbvjq.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/ggghnrlwp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkfpeipd.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gcilfcvre.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsgtxoga.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdfsyoole.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/ghspnizfb.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gshivqmrg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gnvnjoplr.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/geuxjmmij.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnkiidwt.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gknstytkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggprbkamg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjgstdag.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzjwhwql.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbfftopue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdttgemsz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gtijfubpo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/getojodds.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxhvmabm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/grkxuqnoj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjihyqfh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/grshracii.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmjtwei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvatbiakw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwlggmd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkffcjxb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnglsqxsf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkdijlvc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gvfeuwqzn.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/giqgkjmwj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlovussp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grtvsgwqf.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoyodwpl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjypseop.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/guhwcaqhl.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjbrphox.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gviyazwaz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/glsejuqoy.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gucxluqfp.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guxineudp.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjuxehmm.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmeconzxb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grezkgcpk.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfngviksq.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxreamhdv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmltxoji.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/glkawezho.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkhbxph.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gyhetpcjr.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/govnrsate.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdabmzzpu.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxmqojeb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/goofjznlu.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxfyohkjr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdharkiyh.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxcddmtld.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gvuyzqmuv.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxgzxmu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmeuimswa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcizznzw.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gnyoxwzry.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtqpqwhps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gscqzfjme.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gulpfymic.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsddctfm.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gejquleba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grxduwbft.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmiaahzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwruaskcb.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/glxbounuc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guedtrpdc.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gjxgnkdnl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grnoyzvxp.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gkinngmoh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplmmofsw.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpahdqoa.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkucgrrrm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwvgfiyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkyxhocpt.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixpbpfuh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzfqstrsv.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglzfnten.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcyvocgwm.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgbzoaj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/guhoelbyc.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/geatbrmqa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkqzlybl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/grxwydguv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gozazaypy.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrpfncye.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gwnajhvao.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/guxawyhkp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmbeudxq.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gflkcynnm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gsodxdljy.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaimyrwko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdurwfit.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/giqjudote.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeqirzox.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gclyzxcrb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzbznolb.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdvyegea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvnrmkg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqaapprl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gcdzzkzcm.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/goouzltvk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbxxfhr.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/grjaibawm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gupqheonp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgmqknhy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gahembpyc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjglgtas.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwlgtlts.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhrvzmpe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimyipfw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gyonxvoem.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnikpjjrf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgstfmmy.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gohdkykgz.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuhtlvio.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxljuvwqy.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqetgnfeo.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxschsidm.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsfkkgoq.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhnecozt.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gneagzugk.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhlexfno.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwqfmxdk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhlkicmk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gyntbxzmp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/goqzrvdmk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpfkuvjy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grzcxonry.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpzymjrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjrjzydz.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdhpkagr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjxvtygo.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlxvnpca.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmiuwntl.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkjhoswh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikoqwqfw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopzigdzk.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghblxkdjd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/grttozblb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gdsynfypr.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gimizwzwx.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehcezwvc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygwqpkl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gjajgqnex.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzzccyxte.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gceqhppee.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/ggwrujvak.sHtML


<!-- 参考信息 -->