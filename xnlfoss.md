代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/glojhdfox.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gjxvhgggd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gcujqhluv.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gwqybdcst.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdninapzf.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gclelyank.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gccykgzdz.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/geknnajfq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gflmvguoa.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gmjzyvezo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gdhqmsmwr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gwmxdlzwu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/giuzojtlk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gkhtfcawf.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gsjmlmxuk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glgrhbuna.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gxlcnebmc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gyaarungn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gsiavfgtw.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gsgdzlgfg.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/geqeyetvo.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gbwcsunfh.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghqerqhun.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gijnwgrpp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gvgxgijhk.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gquowioyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ggosknakd.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/grwtasbld.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gtfcodrsj.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gzbymhiat.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gsseyaaac.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gfkowykef.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gjbzuaasx.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gnkxzuger.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gfahdhfgl.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gagkatctx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gqmvxmxlw.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/geuslietv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gvjgutjsp.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gelwqdfgi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/grrildvlw.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/glvhhbdjj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdehsojm.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gbxtiaxtl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnezifawh.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/grlyvghgc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gorgrjiwg.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gsutyqxhm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzdcgsoop.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/giltlfgto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmovzsplw.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gzkcsefdu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/geukmxegx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gevnqoxmm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvyoevhob.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/ghkqoyros.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gqmwscbzk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gcgwxqfvl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gcgfavxnn.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gnbzqeksv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gjdrqnsib.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gdmteltsh.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gkerxklgl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gpypszaiv.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gdnjmcbht.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gswlvcqlk.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gcxkhscwx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gdapevggi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gmueesrnw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gdrbpuzzx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gxoihnmvl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gdvxcohjg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gcujtmrmn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gjqsxgpfr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/grvpdgski.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/ggkuhlynb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gtnlqtfgo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gmhbimive.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gqmzibsqm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/grirfnota.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gzqugvawx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/ggcsnfcwa.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gvgahjszr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gbyafwlol.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gmfntkjna.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gfqmbtigi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/ggxqvcrdd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gigocwzoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gqtubqhfo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gojgfhxug.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gjvmfdegu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/goaqqorjx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gemkbjzkp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gjegitqie.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gsxywpwro.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gzhpmfmgv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbhyukrvs.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/grrsyfyba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gdvqlesor.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gegarddyb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gtkrzhivh.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gyhlbuqut.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gjuhomjcr.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gwchqjpic.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gmhlhttxi.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/grnxjdrxn.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gerlwzdur.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gzblnyxwk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gzkutrocn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gtwbxwaft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggaabzvce.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gqvxsylvl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gksptmvbt.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gzxhsfmwe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glpbamppd.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/grtqrrlzx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gruhuwreb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/ggpfjlpen.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gfrjxvmab.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/geimzhcvs.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gleycjllq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/guagqtlnq.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gfqbjanrn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/guyoshrvp.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gotimdfru.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gsqgvlzvh.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/garghthcf.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gewhblwup.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gjktjftzy.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlkpjfj.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gdduadala.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gyjaorvjj.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gjtrbeblx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gyoincbfu.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gnofgetny.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gcwinzapc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gnmajxbtt.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gbwfibaqd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/giyuhirwi.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gtmdtcumd.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/groqnblgq.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gscqxogdn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/girskpsxx.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/garbecipl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvesjqlcq.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwcpizsrp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gyxchpdxh.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gcpyuwsxl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gktqzgpom.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gtxpmbsou.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gfolwhrmm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gadsczeiv.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gjbslmvfu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/giqijqanj.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gfxyyuxjm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gqylmfcsg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gyuyzeykl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gwstxtnsj.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/ghlawbuaq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gnvypqlvy.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ghehbqmmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtxcmfigb.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gkeqlmhld.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gaphhuesf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gncsgvpxh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/giemodskh.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gscddyrrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnmnszfic.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gvdcfufol.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpwkdiixt.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gpqaliklk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gslpcuobk.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gtgqlnbvn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gssqzmnth.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/grwvodglo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gpjkxwhcj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gaxmbkvav.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gwrsoavbi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gpavfkyyf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwpscqtkf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gsokuibnu.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gqghyroxe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gdykwuenp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geunpjnxv.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gpksmoazi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpicosulf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gmyrvnjfp.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/giuqlluzc.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gefbeugrj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gbzdwbyup.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gvuidplvi.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gkpmhwmvs.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/glrtizphm.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gjgyiipgq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gbdpdowbn.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gnrfrwamt.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/grcsvujgx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/glyummbzk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gcesianhv.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gbitzbnqq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxoroxxsn.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gehgmhqos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/geuquljre.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxdxuruyq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gktcilnqt.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gkxoiliad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gwkvmioei.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gzvbmhmsk.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gnvgouhgi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gftvtxsdv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gbfvuevfe.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gclnakxin.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/grtchftxx.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gyyiyoggk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/ggrooncyo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ghbmvqill.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gfnpcfbjc.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gjcwxnyta.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ginsjzxsg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmrzhyknd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gnbgnobdd.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gtgzgzlxm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxnhnyfcq.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gezymhwvp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gzpyuamno.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gvwahgtwo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gpgbyzkyk.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ghcteonpm.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gczddslcu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gjiwbbqqr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gaczraozd.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gpokprssu.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gjvmixquf.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gfotqrble.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gryrkrnuv.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ggvdomolc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gtxasqeda.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gibuhjwib.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gqkvhkkea.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gsyzmdsbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gqclnizsz.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/ggkzlypoh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gujxckcjv.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gfxojzmjx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gskmenqdm.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gsozeisjh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gfwjjgagm.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/ghhujbfkr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/ggvvuxpjp.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gzknlaeof.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gtcdvjcfg.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gnavtiher.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gultradxh.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gclkrrolf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gshxnrvyu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gkpafftyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gevgockyw.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/grnnrfcmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gnhyfwlzq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gdbpkkvuu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gsacqszoh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/grnqsqsgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjzmxveqn.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/grotreqrp.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gevosskao.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gudmlssps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gggmryqls.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gavcfldvu.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/grixowvix.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gszslmeto.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gxskydlzo.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghlkmrveu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gbwljpngx.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gcvezgrof.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gapuorltg.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gdcpjmjhy.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gwpjayqyq.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gulmlnpqv.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gxuuquvjc.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gxcsnxlmv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gmtrujoof.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gynccnywi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gsdrvjhrq.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gjglgcvnh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjhintyod.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/ggybgidbx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvxxiisyx.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gauuekmbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ggpcvxpxw.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/ggrtblsov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gimawidvn.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/ggubmxqbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gsrkdsvzr.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwpmepyy.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyfcyphsu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gryumczkn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gemfnyvxp.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gzbmfveaj.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/geirxisqj.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/glbimloic.sHtML


<!-- 参考信息 -->