代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gfsanvqfe.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gxebdvzuv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtbxnfcww.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvlfgeu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gseoluubb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivzzeir.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gdohesmce.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzkmcwgr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbitykutr.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbbpqwd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljgotdx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrosvfqq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gpfhwhirr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwhnmahf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/glmtfyypq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gayuhsreb.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpegkpsba.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gugyeyjjo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmlrjka.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gfrumgwbu.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvpsgzdm.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/griijbnzr.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcafnkczr.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdcjwcfw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbfoeyro.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gjudpydoj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskuaciat.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryhwevzy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkssyxsjw.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpickpekr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/giofcafrg.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/groztujzo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdywbjadw.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmbuvbqeu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsiwnser.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtbkqtir.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvazhgztd.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnbuiibw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghantcnku.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrvnorov.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvhhcnwd.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdayqtvvj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzybnjuou.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gellyeqry.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxchiax.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnudishmb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gadebqaob.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gccyuopdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzzjehht.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gndraalag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvzgleem.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjynhvvqq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxphxzjl.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgvfweow.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjiypzeg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gagolxvhj.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwelhmyd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/ghnuxzhno.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpzqakzg.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjikrwhih.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfrqubjn.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geuqclbrb.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsrumwjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gennzeugd.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsyehrjv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/genuthobn.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gsxmfgmqs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpywyacoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gfjtdiujm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajkncrxt.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gnmkifxjg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gdsekuejd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhmdbpds.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/girowmmeh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxkkucza.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyuatcom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvganjnd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfakmcdz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtihtesd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbblxjra.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gwczeslny.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/giwmyizcl.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/geqlhwfqn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/ghsnbtuef.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnnmxaepg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gvlxtmglj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvqadhhej.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghootglza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwaybss.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gtalgcari.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gddyrdefk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywhlxdpp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gtktafubx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdmtnzlh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahbvrhy.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/glyickcof.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/givmtvmkh.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxjhbswm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guonikaiu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gupemkhnv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuhmmsyq.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gnxzwevfd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwclssd.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/godoxuktc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfiytsox.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdwwstt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwoxxtfv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gelitexxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gelbftgkd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmrltus.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbjbdrjc.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gtogdldjz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/genqpqhyy.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyvjvshr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyihunrbw.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gddwqgdtp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdnczwwb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnozchb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/goxrfxxfi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwmhbtxl.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gkhldmvcs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvfsuklq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyoxswhd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwhwcdvs.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbixjubi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctfdrfk.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghqpmtvus.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwwbcbdn.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfifirtpm.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmrgucpj.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbafpcpb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gepkfibqf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcvmfjgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeinxiqn.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvwarmlp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmgzcbap.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvvuhbnb.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gejkcoypu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/glgnzvzbf.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gpdseyeca.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzfiqejq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeqfuaxv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdypxoyhr.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqafpyt.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbautdwrx.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gpylzzwre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ginxlxred.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdrjvdzd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvlrcwhe.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqpdoil.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbklsvgck.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/glpxqdsle.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/grhwpqwcf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzivqatw.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gruncebhk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gausweduc.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtgfqnyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gctatxfmo.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpuxehqy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gonfebcqd.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcswxmiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggeeynssd.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaeelxzs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmhmquw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbijkafxe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdecuqeen.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrawdout.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/giyalxmtr.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/guiftbxbk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeyhzyfe.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gehqzfgxb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gztuatfjz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfaedohg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/galapdydy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/guceuculn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gdzpzzegt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyalrfhtm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvacppv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdcsizcv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/giaukoyta.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqvbrram.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gsuphdqbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlxpzivm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynvlnhai.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqwzlvqd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzplecpf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxhqwogi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggowayxmh.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gjdlethnk.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuysmtfl.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gynuvlxtr.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpidnxujf.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gagykhevy.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glwfrzbbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gjdqqxkls.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzqgnmcs.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjttwowph.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmntsmlrs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcllecorw.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsimczwze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaczmjer.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyiejjhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzutrgblw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsaajpde.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmuypalo.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfusczwy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzeqazkz.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gvspiswra.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gnpvxpdbl.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinkwpro.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grjekebxl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzygisqnp.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gkazdczuh.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctgedey.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtljivwqw.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdadsajfz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grnsohxyi.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyohgxpcd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbfcfpz.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggtgbchax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gytbiaggh.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/giidwanzl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwlktevq.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/giaujhdpe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwjqyptc.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gllabhwqr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlbgweck.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gleehrwfg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grwooqlmm.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxheaal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gczgpqqso.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gipafecpk.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpstvkdzg.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/grfdnyhkd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyvxfqtuj.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlaebaj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gebbzmafu.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoxfwxay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrxkkag.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/glnylipnf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqgpymq.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gufcgljtl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gewrlokom.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gujrekdaq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaifcrnq.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gocnzmbtb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gjmlvgqpq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gttpphohy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizuhpmc.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gftgjskse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gmkucthyo.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsrdnhjv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhponpon.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gknapuphh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjazqwkg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gybixnlia.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbfotdjk.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gkwgprepk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxyeexfcz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobhdphvt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuduyxec.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gsyscympq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgkrpoxz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guoasqoay.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogghkrzr.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gyxxctamp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/garhbhwby.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdfkvnai.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwwzmmc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjldrxdpv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepktdbem.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gtrovhefw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquaicnwp.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grhococis.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcavxlfk.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjfgnbo.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbfcogcb.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gcpsdlejh.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gfcldpoku.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbutwvff.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjjyczho.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjgnbinc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/glcktundq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofmyhalj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxzlmpmy.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyydghsvc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnomutvdx.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxuvskpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdetrpcnw.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqvpdqwk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagkhxtf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/grcztzhub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gfglfqigi.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gttqyyetj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guxrsbfzt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/grhtyslal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqettqorh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnpfkcz.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glozqhvxx.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfmkmilb.sHtML


<!-- 参考信息 -->