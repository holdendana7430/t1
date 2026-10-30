代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfpdyjpg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gufuekhin.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gmwfrtvet.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gvwerrrbi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gndiqsagl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/grejavskh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkfncjxu.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtecvwgbz.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gjgzztsre.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gxjwvmqzz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gvruefmvt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gttybvpox.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsmgzftn.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeiuntzl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyidwaxq.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gvuumxghl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/ghzdzdyja.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gtmhqyomj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gkedhxfma.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkxhixbr.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzopqpzx.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfubhepjp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqvymocn.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjtkkyqwo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrplcmbh.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwikzrfw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gbimcfdid.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gitzwhdog.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwjmzsmv.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykxvgaie.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndsojiui.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvrnpusc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxauyyxl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusuhaop.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwggveetn.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/grjstqhrz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gwwxrunqt.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoruzqib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsqzxssv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlcnlmrc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gkascejtt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdgtoic.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmvapkn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ghtnrqovh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/ghejtdckg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqajoxn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/ghyefkkgy.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gkibjvslj.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gckxmebhe.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gppjcqkgo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbzjnbvh.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gboddmzpy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grjimwjas.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gytxeucyc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gpmhrgfop.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gdfimdind.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeacukgo.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzcfjtwy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjdhpjyq.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gzkyvpzpn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gbobqasro.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gylhqsnql.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gayaycxqz.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gnemhkota.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmuqfibu.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gyscfrxtn.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvenhry.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpysujuqh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gtjmsfgpt.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/goktpbeaq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gulqaxzfe.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gjbuhsdbm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyiijoji.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhvkraga.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpumibyjv.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/govjjjvce.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdamlxuu.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gktwmgzkp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gpkvyzgho.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkyqosc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxanrcdgk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gshcqvbwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvebhsegw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/ggelmjdtm.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsognoibu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gfnjemntc.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gywpbquuh.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gevnwtuej.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gdckqibwo.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnynezxlp.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghssrviqb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpnvccsv.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdqeqmoqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniivlmll.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghitixqgp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gyevyruyp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/ggkekkubb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gauhnoxyo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gtilfucft.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/ghruxqrbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gkqsnacaj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/giuyldsfu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxaewjaw.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsviyzqp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gyfdcjckl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/ghenqbhei.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxapzob.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxlioioa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gfljcvwda.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggryxzqwm.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/grxkfxhwt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfvznfpv.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsolpkuco.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/goqfbylpw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxewzdjqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjjaxucm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwjwowykl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gurqugwls.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grewdmopr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcvdvdkv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gijnyjexl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzefowyk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gknwcqlyc.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjvryykg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvhmvgxs.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmjddmqo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqlimavp.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gxkdakzym.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbirfftk.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwdhtsxf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaeukplt.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghcbmutji.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnymftrp.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gliuvfeqp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxixuqsp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbotjlqud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gwifapdjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/goujkspzn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gulvypcpx.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxhxusr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkrmclzx.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyaewcdm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqbglcz.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/giwfvmwdt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnjdsxca.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhuyrnvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgozxzsd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahioclwq.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gitxtuwyr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxszsll.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywxhuuo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbtgunv.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeqnluws.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqcohopv.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghodpgucf.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/grusjermy.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamufibbz.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjikhon.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gcphpdepx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkcaaihy.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/grqjfyprd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwpqeub.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwdaqaqp.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyookvqm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwkthfypb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazljxgiv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrtovgsq.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gxvwcmeuc.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsmczys.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gddglaboa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazxszlgb.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggcikzrtq.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjeapzyxz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gddmeleea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gguahtkuy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohoiaxma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspqogwcm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcekollrd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geklndcku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwtqiouu.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzytimfu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfpcqhvp.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkogjechz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gwhlrrmvh.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gerstiggu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfvonjzj.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqwxsugs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gosahgwjz.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdmscidl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpljontw.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnsordzr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grvgsicpg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdbjqzmm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojcefomy.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grzhlrpsf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gksksrlhl.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapzpbeub.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goivturof.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gapmsbzll.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqbfdlj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvhxnxjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gudiunifb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsibuuwxx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcprozxbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gxtsbtfqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmvywds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/geutuhmeq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gonfmvhjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrhifoz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtgbonws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsdklzdu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcouwhedn.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/godvauatx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmzoktucg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtktjzwh.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcfhuooo.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtrhmfce.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkcojyef.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gpbxnizmm.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpksacpow.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gvaumgecg.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzevpasko.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftxylbif.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqxalfmyv.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhoaihf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlduipuw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glofhutsc.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gffosqxkt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjnhpkzml.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlbpasag.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpiuzpun.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghwzbydie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtqmzco.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqagtxzgm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbqyfnmk.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gnbabwzgi.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqxpjnbl.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/goovivqmm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgqvxvll.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsutaxzj.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslehwvhk.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvsahilr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvjfoqubo.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywqbnxhh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwrzpmjo.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gkboknbup.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoafxwhd.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gypxubqbm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkxrllbp.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gappddmsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbffpqoij.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvlkiyew.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrizrzpp.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gwjyeufnl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/giptlwzei.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmnzddxa.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggozhaatp.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gtetiwxqs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsewwbhge.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdgyazu.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrsrbyui.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/guxjjlxuh.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeuetgdt.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkmxybcc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gaqomquur.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwomfyql.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxfkamh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gmcloxdpo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmyskzl.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/grgzfhuvw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gkpuwvkhh.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcxaoqmn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gkoodzzmw.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gacemhgor.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ghclkrjrt.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gocddgkap.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwchadaqs.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdbjvzmfr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gglfaleeu.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvcuwneci.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgzhnzbs.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlzpqfa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gylppawdd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbcwxaest.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gvjpybbis.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/ggazygjzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbpxhwfq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwdbpmye.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhgbzwkf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gempiimhk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwpwwlm.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqdiznkxk.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyxxnxt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gaefhzlpt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gugtbnekv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbuotcex.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtwgwtlr.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gusebflap.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gcpybevbg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqrwahpi.sHtML


<!-- 参考信息 -->