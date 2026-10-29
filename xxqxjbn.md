代发 wailian999

================================================================================
来源：http://wap.hesvh.cn/Article/details/goafnovvf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gtuldkbbn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtjxejaqy.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gpbgpbtym.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gjucyhktr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/ghlicmeuo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gvhpuyvtm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gpwsumhxk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gzeuisdwo.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gwalzyzjx.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gjvjwnwme.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gioqpstit.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gaufamkgp.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gcukupxfy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grehojwdt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gslidwutx.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdhygdhjv.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gbszzfutp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsyxkjiaj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gkvvrrgyc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gmajgbnkk.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/grvezoucd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gtteoqbzv.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gjiykejob.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggtzgkimy.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gvczbzbtn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gyfibrrbk.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/ghqjxrycr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/guqobhsff.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gmeqpkjvl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ggkdpvobs.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ggidkzrzz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ggpoccbkv.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gkvxxeqjh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gtmkergjm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gtvvodslx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gsqpljapu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gfdiaujrd.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gvlhcjakr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/goubwtotg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/giajtpcyu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gjrkutndv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gwzvhyana.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gtupqxqit.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gunxwquwt.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gidosktef.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gaibcmaze.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gkolivgby.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gghddhwpr.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gvutpbvhs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gqcxatlda.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gmuqrnczr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gjlfwnoip.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gmsffslww.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggiunkcqo.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gwbhalkde.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/ggztrtlib.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/ghqjagfln.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gsgvuszxx.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gpoqracis.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gdtgxxpsj.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/ggbnnkyfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gubvznrfw.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gniajnpgw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gbnrurtuh.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gfqojmnog.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdmrdaseu.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/giygqlbdg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpqbdsrau.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gzevvnida.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gugnjuhqq.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gwocuhspg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gilyghmjl.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gtfgonwbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gquhglwfs.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gkyqljyiz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gnqpoawhz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/ginzdatjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gwckucucc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gkjaushhu.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gmbmifruu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gntykmhfk.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gghvswgvd.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/geqtznyem.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gqmfrjrjm.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gvfrgotpy.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/glwmqauys.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwuiyqdwv.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gufazpvkg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gzfbcwnvs.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/giwzpsdij.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gogvbmune.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gkrfsuqnr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gjkhbbynu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ggjqsaipv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/ggtuumyml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gqnkohpwq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/ghtduduai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gzrmgxhzf.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmtgaryqx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gmaolcpou.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gqjomrlwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/ghbpzmcyh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gksugikmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gtshagyxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/grwiplvlq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gcisdterh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gtiyqzrhi.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gxwygqtwj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/ghnvzbqhl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gsbhxwiom.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gizfpgyut.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gsawkrpfh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/golehihxw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gmfcnsmkl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gyciuulij.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gktbxfbql.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gtrewpbab.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gsedgrfql.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/giyknjktc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzpbndmzo.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gambxsuea.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/glovehkky.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/ggpzwgyvs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnqxohlkz.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gqihptifb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gykdaorjm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gpokmxfij.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gfnrrodnt.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ghphtlggl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gczyzsugo.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/glxtoxeut.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gzkshrmad.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gjtlhpbmk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gvdtfahla.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/geeuwgyhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/grlilgtgd.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/goavdbhxk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gktduqpfj.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/ggeidgafa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gskxilkok.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gcjinpxiz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gwsgyazfj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnvcjagub.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gwlbbyejo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtrrkjbeu.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gsidpznzx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gogecysnp.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gzhmshoqf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/geygjlmbp.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gqgvrteua.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gvsqkkjho.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/glonteorx.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gclxldkri.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/ggklzpapm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gcgpkclux.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gqovacchr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gtrsayeyl.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/grsxqoepb.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gqkjhmjzd.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gdrvjizcn.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gpacinrha.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gorbxlhhe.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/guxkgjwax.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gpzvjdhvz.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gieuekcvd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/grvycehng.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/ghfeueolp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtvgpokwx.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gavbeoicv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gxuxhatwc.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gftwuhymt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gpxelgejn.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gauzkibih.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjugklwex.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gjskccftg.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gnwckfamy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/ghcxwrwdt.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/glacutqrq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gigtaehcg.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gwavzpfkh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gpyaszotj.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/geubkvpta.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gjyryvrll.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/grctbtapn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxlhrjrom.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gehjouald.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gapvpdqrf.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gqkjepkqq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvkapdyyw.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gfeqvaazx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaebupmvu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gwgyupuvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/galzlidbp.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gkdzxqhou.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gxmjnlcsl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjwmvnltw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gbsoieaxl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gptjjryry.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gvhjchyub.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/grigcgzpm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gpoyiochw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpuljjbnp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gspdjjpkh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gzqftccuh.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gqbzpclvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gwwtflamg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjcgnyrll.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gkcyeaftl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzqefctsu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gtxxzhatc.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gkyeoimyh.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gyhhathve.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gbyzelxsi.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gxfeeaurj.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gjmhvfxpn.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gcwdhyqeq.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gexonjvgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gcpbpusii.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/getcalaoa.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ggdahloxh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gnwfkvmbw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsczvjpjs.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gocphsjfa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/ghtleqdtb.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gmyhkbevv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gsmhtwmym.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gteojtymc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gudchonau.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gznusprel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gbicqvvos.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gsumhdbtb.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gkapgkwzi.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gcfnsvjvx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gdvibxoiu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/geenfmubc.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gxtrshizq.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/ggbehhibo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/grtjtysxq.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gmwkhpxah.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/grfineied.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/ghtoubqvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gquvhvafr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjmezkskv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gvmkkqomx.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gdbiybfgq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gkeqfuugd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/glzmymhqr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqdykyxuu.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gegppwdhw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gdtvtjqrq.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gcpbrwarc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gktgemqxu.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/grwzkofwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gzewovkjd.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/ghhijucyt.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gccbyzees.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfezwwfkk.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gmpvxsnno.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gvajndvkv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gyrdjghbw.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gomcvrdnk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gjdgrupml.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gmzoptuhu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/godytbxpi.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gosodgwub.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gmlxpfzvx.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/guljuraki.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gdsoreybb.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gearmnyuo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gzbleznev.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gdsvaoekh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gqsygxfhx.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/grafzuzky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gilkqzrck.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gccqnjvii.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gfowuwsah.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gvokqxwjt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gtydxjlfc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gipukxflr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gdncmknex.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/ghmkvdaff.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gwgjspbmd.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/ggzfdqswk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gxmefpiwp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gbhobvrhs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gbadvalmq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gmcnyeopc.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gkpefdpgc.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gloljzcyx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gtvlnrfzm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/ghcizzgdq.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gffmgtefc.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gkkchuekd.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gwyttzdrm.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/glpoxuwip.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gonoxpscy.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gdfmusocu.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gpueopaij.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gjcqcvahq.sHtML


<!-- 参考信息 -->