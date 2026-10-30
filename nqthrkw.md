代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gsenffeyy.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gfurqisrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gsyqxmwiq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjjbfkk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gvkagpedd.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gcaaufcti.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gtgarniiq.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfqaeyg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gtofmgair.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gacsrfahx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/guzxcsrmm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/glgtyjjjg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gzgwlxknn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gwdzysyte.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/geqhysqjg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gafxsbqin.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gjyategir.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/geldxqjsw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gisrlpwqs.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gkqikcnqf.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdyugsvfe.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gzoeyqkkf.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gwimywqlh.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gbcpwmawv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/grfrjiqqu.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gzqkfkqki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gdxzbwrzk.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gzkylgrcq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gzkrmeixf.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ggztogvqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/grugnypmw.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gaitoulgh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gfscmuciu.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gybusgvrt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/grxogfzsr.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gkahmxtww.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gxgmftdhg.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gclzwicct.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gllgmdpnq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gexgymoah.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/govznlilp.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gbcdtkasm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpemiuniy.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gvbrejxzq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/grctywxjp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgsoyky.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/giwfavgmg.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gaknheptz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvzscngsr.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gdoskfvag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gwfbxappa.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gcsutvppf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gftbtkpey.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glnmpsspk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ggppinlub.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gbosukjot.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gyszgaifi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gjypikhky.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gjkusqkzz.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/ghppnxico.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/giizbdpys.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdkdhaypg.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmeialleb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxgyyuqkp.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gqmupmstd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gicibogek.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gcmujvagu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gcnqprxei.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gdiftsfpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gclahisdl.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gqoglxhvi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gpcybhxze.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/glwqgaedq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/ghgxtymky.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gwgbeitbc.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gjgybilmy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gfbkmbyfw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gwaxlllak.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghrimpgni.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkvbkhinv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/grdmbftky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/grmqqobmi.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gnfljcrvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gkepofqvx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gpmlghaqs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gihrwingl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gltduqopl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gjrzyidil.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gelctdvcc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/giejwqcju.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gqkgriagn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gnwnlsrga.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gltltuexe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gfwukuehu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gtwwajixh.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/ghirfobcv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gjasroyrp.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gfuithesh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqyviziym.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gczomodbo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gcyxstgvq.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gkrwlmkye.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzpxyjpwt.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gbnajkgxg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gxcbtuiue.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gyybtaquh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gsbiglpst.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gmxgjjedn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gzmisepwx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gosnkwwrp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gsetapngl.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gaqvmffiw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjaxsfywc.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gtjgiorif.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grwlmgqra.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gtywxammc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grhdtxyzj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gfdqctzbr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gsneduigs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdnbrkpwa.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/guuqbcfpl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjjkococg.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/goplvjmzo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gafcwnoho.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gixkktaba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/ganhkoqlm.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gczpboful.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gznlzmuet.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/glmemgsxh.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gxchbinli.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gmgregzjo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gxkrueflj.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gsyzjhfbm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gankjabgd.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gndqkszcn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gypctgodb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gpndtjhkf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gtrusyxoj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gpfssudbl.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/ggrowvjwp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gueltplyf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/ghzzhaejw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gujtbxbwy.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gzkedlruf.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gajwwgsic.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gqeeyxujj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gheqaadwp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/ggvfufeeo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/glcdgyoph.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gydqtzqfj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gndodrgqr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/ghwjunitk.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gaxyivkri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gcorbdmsm.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gxdwbzalx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gfwlungzj.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gkxmvejkx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gosxnxjrz.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gnwmznqzu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gzzaircjj.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gfefslyyr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glvsmfawi.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gxnircvhy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gvgupuvtw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gaemwzcwd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghbtwdxat.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gpahraayw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqgthocou.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gkrhkubge.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gahgdbvek.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gjryfinvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/grtkinpyc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gxsmmovdl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gcqiuwodw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gotiafsbt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gwpyloioc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ghymtzvqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gauynvfxb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpowrcabg.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gcnyynnin.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gaftplhhx.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gpnllukyk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gjcsuoxdz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gudmvjeno.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdeqjynft.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjpdztwmf.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/guqcobwas.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gvesxbdhj.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gnlengrhu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gdbxamtsb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdwpnsg.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gijwffzje.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/guegtynje.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gcckbweyc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gfqhvwfba.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/geyrddmai.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gauaefgqy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gftvludud.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqglebmwl.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ghfercdju.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gfaabfoek.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gzitvgfgf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gmnbgiwii.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gstqtguqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gppwevnnv.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gsvazboct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gulklbsog.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gplbdacso.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gtosohxax.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfsyydxuc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gazbvlvjs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/guzdidahf.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gozviwubp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gdtcjvfbf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gckeuzaxw.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/goufmtvaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gdmwqdwyw.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gmwmfmdvw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkgsninkt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfqkbmllh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gcfvnfcnr.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gqzkuftok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gpsangktf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/genmzchac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gravflgmw.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ghspqffkv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gebuqosyx.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gheyfwbpf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjuuvqnoc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gwjwhhewa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gbjmtapnt.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/ggrjxgyss.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gzueavylv.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/godjuraar.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/guxhdnqou.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ghescveer.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gqgnibujc.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gbyijcuuw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gogvpmikz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gxdejydcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gqtwdnysl.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gupqxjwqh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gecnimxiq.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gjtcbbzrd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/ggpcamgjd.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gmtrvtocz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gaqgczbgo.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/girvrxyls.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gyqwgrpnh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/guxklshjm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gbgpoelco.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqfkvjxyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gmnduhwqn.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gmtzoyowp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gpjzphyhc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gcghqvaxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gvaptqkbl.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gtojvrmbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gojddcmht.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gniozkdxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gvottciqr.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gbulakudd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gnfreends.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gfgfatkfn.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/glnejvhfw.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gdnozvkab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gpxdrmzrh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/ggifgiaue.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gaxyoqsyb.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gagzvvlqx.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gzdkacocu.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gxpaclozf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gnqrkukae.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gxvyofpjh.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ghdqhmufb.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gcenzwbuv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtggrxxgk.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gvmacxzgd.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/giwfznyyx.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/grkpysxja.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gkhqbrcko.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gvwqtnvsi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/guhvmnzrq.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gaewtnzra.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gukujhgtv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/guoheozkq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwkynxdnu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/glefmajon.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gmmxrarbz.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gbwtlrljy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpysvmmwu.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gzsvdxpww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gswicwvbj.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/glbjptjuf.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ggoywmuoe.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gqnbrpxvb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gtqzbuqyw.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gbjpxuwkl.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gmzxqeyne.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/guevwtrki.sHtML


<!-- 参考信息 -->