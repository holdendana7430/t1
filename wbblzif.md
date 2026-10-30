代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtcmcmi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdfnlcd.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gktmtietl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxxthyfn.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gslysxfxj.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/goqtrmnum.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnfzraqf.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbiyymh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkbcsjc.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmatgyhtb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutojqipz.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzulsyct.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsmpgctl.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/govnkdcww.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpsoiuao.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gnselnbqa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gejozyetp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrmoiek.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnrrppch.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqoxefgq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsekess.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gkibygaxu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gepnmqozp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpqbrjvv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gyqkaznys.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gsywvlhem.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gqunmxjty.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gczoxwveb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gftzjddgu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbonijpp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/grjptfxzr.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqgznovj.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpsuakvfa.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/guurjizea.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsfoipinw.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljxxpkxu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gydvasccm.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbrqgtsls.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/grsvqasfn.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxdvaxplw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfzjllvx.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gnazvnuqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnapzzxwh.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/guvxbtwoh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwedydwyh.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gseadnpjo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gelbzomkt.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqprsoqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gvqnatjfk.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gckyzzmjy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gapdjuwtp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gvypvyfzm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gulxknggv.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gycikehax.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtkyruxm.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gosniunbf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwplayp.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrrjnotz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjenthbw.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gwwdltyab.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlykokhi.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gwvgxwcgt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvbjhjse.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvecwdxad.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexrvdmzf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfeiruin.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwbyhjln.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gnhfeinze.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gecuuqtly.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkinyoadx.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/giizewbhv.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gjprteivf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gkwckfhjy.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzygykmj.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gkrmrpilw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwggecyu.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/grgffmwwi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkigrkls.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gygbqhmqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgcyhxev.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gllhlcnmj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajkjuqg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvyawpff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gielmnzao.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/govejdhoy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gkjiyccqk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocesqhlh.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmqtgdake.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gybvieimv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/glwkjyzcd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtwjilvv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkepjztmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfubrqzi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyasstfw.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/grcqunbch.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gpchzeyyf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giunvgvkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gudzmqfrg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsyiqwwva.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/giigshiuu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeobhhiz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosspepn.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdspregb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtjfplx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuonquxy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gueasbori.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddgrmyq.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gjlecsgce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzznqoem.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxubxvoiz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grivnnyjk.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqhatufs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgkqgvgv.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gmcbpslkx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfghfccwo.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqkkblvw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gvkzjedww.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbybspg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkshyiyk.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfipkaa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gyiffxfzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gqmxiecul.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdltpxzp.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqdqqzxf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjrgojic.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpbhvnre.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gleechafb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyopjbzi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gthtgwsdj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfzwmgdt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhczebr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqsynevv.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gfophmclc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glxlxfcxu.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/guidnxxly.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/glrzwcywn.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmfhwwjw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibtbjpbe.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjhpyimvh.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpeathc.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpweujwbp.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghavcjpmp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwujmrmh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsroedbf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfhwnytp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvppwjvu.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/ggzkgqfwm.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/goxqtjcss.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbopbylko.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkucmmonr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gmwzjhstl.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqhnrpsr.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gibxhhsrt.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuxvioro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gokhmhmmk.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrjwytkg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxckxmcw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzfqrfiv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghlmktgfk.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwzzjmcgn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gvteugdij.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmnknntzb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grnnsrtwp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaprsyif.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gyduhlzkp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxtvcxzi.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjusuedm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gaodjnvem.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtvbvodzl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gjgxdthoj.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gypnufczx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gusocwppg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzmwiqon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gepnjnrcb.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gapfeeell.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmbpfqrne.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbinroxvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfebciti.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gulsriyoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvrrsaaiw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvhnjzkl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnhlnobr.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gjwsazixf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvybbxf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpnpighw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grvqpwwwe.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnpwqzkw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdukhmgso.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbbdyksj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gkizfhhfb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guweqxqaa.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfyihannk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjyfyjku.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gdkdcdtsv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoyzeznf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztxhorh.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gcmwysdwg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqekkzsqq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkljwnnnw.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrjkkkkd.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbruslwe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnfbzrj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxvqmows.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giodculir.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gdndzsndu.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwmriudxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgrpauli.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gdrzximxf.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkjgulac.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqolxyc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guddndacc.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzwftzfxe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamwegkiw.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoarxdxk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbsaalrx.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqoxace.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqesbkbg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdhmdzaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkyxzbyq.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/grninmpct.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjcvkjyo.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjagedez.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbwybzvg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gulyiikcv.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/guhidnfjf.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnvremdsv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeyrkkqv.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizcxwqtt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwedhlvdv.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpflfuxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfuxwerc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gajesifbr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsosjgbji.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzdkuxvp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghubprvyr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glffnsfro.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/greqpfqvd.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnpgxpwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnouzuonb.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdkchpivk.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvfuedrf.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/ggdcwtljx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgfnxgvf.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gudnqxlfn.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuvvimkr.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcubwiqh.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmgteeh.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grrgdzxcp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhsflwvh.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmusjkkn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzysnlg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxxdwtj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/groiddsod.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfulplumv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gjesxmwtv.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gmhhagfvy.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyarmykc.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/grbtlrbnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gjahuerak.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaddadoro.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gahznjlpj.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqmgobsw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguzuykcq.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmrhctu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gftcwlvgm.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gohbmxixk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqkhpjqd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrhzttj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqsxengb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhlyomz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwgnslwvl.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/grhxxayuf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glorwzcwy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcwiodpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gidrctwct.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfetbvdke.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydprofah.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ggpygfeoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioavhtz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gahrpmgbw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwmjbkeaw.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gswmbqliy.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqcwwmqq.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvakhtebg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/guyugixql.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkvnhrtj.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkqgkdoqj.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gobpkjqje.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtwrasujw.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gchcdddym.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gankbqntl.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwtoizef.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdvauquc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjsvimzy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gdgidpeqk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybmsstkk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsxagxlu.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gkbohjplp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwxagthq.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnyqdddty.sHtML


<!-- 参考信息 -->