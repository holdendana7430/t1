代发 wailian999

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxtgckaj.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnrconsk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskkhrbwa.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqevittxq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpheoluod.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqflxaho.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/grhkondra.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvfroraf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gqvsslarb.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gmpvhmzen.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlegzypm.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gafnenivz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gyxvfrtgo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gqapuavxo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxgjltix.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunwzdvrv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gygptarze.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegaklxrz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivbkkkx.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gmjwxhcwv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttmasgjl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsyhleed.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gxokqrgvs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/grcnrwoit.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjoeekg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyqftysk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnujbcgnz.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtkdqzl.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyorybwnq.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gojnobxfl.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grcorfrxc.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gscsxmbgt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcrewsdr.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmcyrsrxm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gcxnvfncm.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbxcwungj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqtvmuid.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaojjvat.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnockrqq.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/glcspkzyf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsvxucyv.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/geotlfvus.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gwoexuazr.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/glouqgdnc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/geqboghtz.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gbofaefcg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqgtmzyy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmthjcq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyostlqo.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/griusxikr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geqywgdlq.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gbhsfmoeo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gevawrqhu.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gmlhvjjtm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyrthgjd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyfqktuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeavoplo.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gabvspoah.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/guezthkda.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/grokysxqn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzzaidcg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuupdxci.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrmoizo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gpbdumfuw.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxplmatp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girsedjxk.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gqptptxjv.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmecwuet.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gthbrmkjj.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeqcwrvz.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gslekkyko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxanqqmaa.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxtgoix.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzjbnrpk.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gzwsxxarx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdretyehz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiurieln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbvuvwt.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/goespqvap.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gfevprnph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/ggfmvaezu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcynvocxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrjumjsx.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/giwljkxwr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsedijyo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gtluwrdzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnnrsvqs.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gygbpwpfo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkctofvmv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gahphjnyh.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gdzybjbom.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/girugipqz.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gftjxstqa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gypysatqm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkcgzejv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawexogxc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnudzkkxh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gzoimzdda.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvyuitid.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbjwggky.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyrdtbve.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gopjlwsjt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/guewqwiei.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnafhhy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gsmpvwwxi.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxmfmlfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdnseijyt.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gaywrfeos.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gilefzkou.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/guprcvbui.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfzysgsi.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/glwoxcraa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzphpcso.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfthsdo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjbmyepb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gctgcrhse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbdgzvhw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gnoxvhoja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllrhuujh.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkqaxbuq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glngqgmrb.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gidjkmpgt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbwkdphsg.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnjcckfz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqqissm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhetpzvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gsluspoqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajmiihm.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnsaoefv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbtvwmuo.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxsroqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gxponrloe.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwazpeqrn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gibcnrzqq.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozdmnfbg.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtbfyal.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrspwhs.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/glsutjtgt.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbpccsqmc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/geutgmhsg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqnohqqb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gaplunmsc.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gvywinhzt.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gydicwhxi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurycjseo.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuqtdmvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeretfbc.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/givpotpjs.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfmapoqew.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gablkkxko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gsknlhnmz.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmirvqtj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooutippr.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gfgojqdnz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsfzrspp.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnwejbnx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljjqxifm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjzpzjri.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gusrzyeew.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gmksjzpkz.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfmatng.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gzbvbwypd.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/guwdbisqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhphpnxq.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gzmbbuyki.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcherhbf.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtngrlj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gcwaavoot.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gtfegpdmy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guejaodru.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfniibbry.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdhosnq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlmqtkyz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgzndacs.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gluntefqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsziofsdv.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gxlqknfwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwyywyluj.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkabdnjn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfogarmqy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwifbrlu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrcpsal.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwdvajso.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltbahiy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxhmitc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/giywlurkk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdfwluqe.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gajkfqlhc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjyukyhl.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gfjiuyvnt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmagcuqfw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gupltsfzu.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbonvzknf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gknjwpuek.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gtuocywic.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcfplrpa.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gkjqvvwpw.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gfomzqifr.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gpzsctljy.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/grhrxnvth.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gbsspbpmj.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiilraqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gejtmcohv.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gutrvyded.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofhggba.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkdouvtaw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngbmkwak.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/grupkxhgg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gocjoowat.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyxtriggm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gamklfuuu.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guucwhfcp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghteojew.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvttvxsp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdewghauj.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gddideycu.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejcalnow.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsdtziio.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gefpqooll.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwifmtqhg.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gwotiqohx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkdqgure.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gexqoxeoy.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjcipjmg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnakuhik.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gahfcjedv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gffgswzno.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvrcbmol.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grzgkaprh.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/grwdwrqoq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmataova.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlclvthh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdenswop.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoadcfna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghccpnkva.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrrtvcr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjcukezo.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlxwzfq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/govttfgzl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpnxsyqx.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfbygblda.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwunflwj.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbrxpkacy.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glelvhkzl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpmdacrz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmvydsikx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gofphymal.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmjpjknx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevaxxhuk.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gijupmapx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gncxjlzlp.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gylmeyzlx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnwxyzc.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjazffgea.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/goktvpbzx.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghozbkcvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gujhzejrj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwrjwzbr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnvpqdmv.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmyucji.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyihyekkm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxsvnpte.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggeubgadd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/grigmswli.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwjfejui.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gvcimlwni.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqfjrrbk.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gnthnxkmx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gkofaynyg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdegjuksg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gysfyikxf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gazcvkfop.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavocwmle.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gwshqaiew.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjzvzezh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gezjswpqz.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ghvwklxhb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrorvbhm.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjabqfaj.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwkdeuh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugkafan.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpciyjyyu.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrmhvgdu.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gktmogiwf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpknovqw.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsjorzlhg.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gphllwbuq.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejglkgc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gstounugp.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gbpnqbleq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerlfiqbm.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxhpbul.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gehzjofps.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqhboubg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxpjhxgea.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzgoguxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakhteyih.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gteaxlkua.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grjocaojn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gyvkpocxh.sHtML


<!-- 参考信息 -->