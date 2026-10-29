代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gbwwkxwok.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gkicjrcmj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gmtubsmqg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gohkdvxry.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzgvqtrru.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gjavwcdog.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gslxtqgql.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gpsfstyrx.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gtzltrwdg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gbqdgijzc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gmxoxznwp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gsuazvcrx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gyqfzclzn.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gtbkxuntx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gjchloqdi.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gevmehjzx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdxmpxloc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gktmsmkur.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gcwaorbcu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gghhtrkhb.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ganmmbbut.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gcgttftyd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gumjkclib.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/guyzlpawj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gmcbajqxk.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gylqsbvbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gtdfkbthz.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/ghfnjdnov.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/ghcfxlqns.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gtfdlcagf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gkqqkjizf.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/goqvayqge.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gpakyxyej.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gdaltwtgq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gxxzjmsyo.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gytsnbdmt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gyppdgctk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gybbqhcml.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gpxygghof.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gnsgrpnir.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gjhjlqwat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gfeowzynz.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gqwgyoynz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghwogyoyb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gylgwncqx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gheqomlmh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gvkvxciwg.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gqjeuypzy.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gpkzwhijo.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gdzpnawrv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmtoncowu.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gwymzebug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gtuhgjbik.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gsnacbarn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gvtkkbycs.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gjxnizouq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gwytwfxom.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/guxlrfyft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gsiumisad.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/ggmeuclrq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/grocmokcc.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gjpullmtt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gjrdjhgvi.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gxgcbpjdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gdvvnszlx.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzoxrmjff.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghzxjydgw.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gktbtexwz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gjrwjlqkp.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gprlgwduo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gektwfjft.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gosuohsis.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glwqfzwsq.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gotiddywe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghqhjqpwj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gbcbtaxuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhnsxyv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gzcdqhfkb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gruxyysjj.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gcpswauke.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/glierzlcu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkwkqjjrj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqddxct.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gffoqpeih.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/getqcmrbj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gnafkfcqp.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/geekinifk.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gttnkslap.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ghgknvshj.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gudhwxfvc.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/getodwjqe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gsrwtjsap.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/guwplywxr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/glqfxximu.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gpbbzsnur.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gwuxnqvfc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/grpoxaxsj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gaeecausb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gwlxmreiv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gotcoasot.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfpzyvidx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gqaawzkkd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gnogqgreb.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gtqhtrgzb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gmdfdzehs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gtsxcqugi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gpvkrcwzr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gckzadbul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/ggrahnulu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gvxwomffa.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/ghsmubgtj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gvfbfmtym.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gtgtozmjd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gmjupprhb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gnktrlbdi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gbvbhstfp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gerwnqexo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/grkczywpc.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gdauwblrz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/growhlctv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gsgoqdxyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gefpgeygr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gkztotlmk.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gxqpuhykn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gshowbnkb.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gsgkycvsx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gfnlbwlwk.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/grxauggyy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzjfunqxa.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gldjnnqao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gngbypwjx.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gtlcgzfbf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gksgggeyy.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/goaooxmvm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/goddlmebd.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gprvkcfzv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gswksalge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gvgwztpoc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gubxhtlsi.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/griopjxsb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfkyuhmfr.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gfbifnyha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gliesjjqx.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gyikfepym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqatsfrav.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbotdildt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gwvxnizki.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gukgfvumw.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjhcorkyq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtjilktvu.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gwndffogx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsshqgjjh.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gxvqesdxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxfzykwyf.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gkutmnoaj.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gmwacvsfi.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gkundmrkw.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gmhxbsadq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gvsaeisyp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gknjhiijr.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gxywutled.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gzwglsvsl.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gverhjgzv.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/goeevtjar.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gptisdhir.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gyemkvsss.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gqbdhkqni.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/grhbkgpjm.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gjvbprjyi.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gotgsljgq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gxoczdqbp.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gbgfvdrve.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gncbzdije.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gfmstrrrt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gyoerwivu.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gtvvyixrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gbgcllwdm.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkytbojxg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfiovedrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gvmwjqqdz.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gkbrrsraa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gyqjhzmcp.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gxmmdrqpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/ghbmotxnj.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gevzagiot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gfglphpoi.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gpsfrooah.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gpagxmavq.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gzmpsynok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gitxucghh.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gwjuoocvy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpntocrqj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gaqkroysi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwctadpgv.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/galebtrxt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfkqdipmc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/glbqkaqka.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsckuedkj.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gietladmi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/glhooboxq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gwlmjayzv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gwdowsgoo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gtktuhqvz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/ggsqrnbnd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gbhzedeix.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gwchioved.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gzdimwvue.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ghbogqutd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ggnflqjlh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gvscuvrpz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gwuijtixm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwgbqmilr.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gcufcdfwc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmdeltpxw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gxskidbco.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gcjhzczpt.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gyjyartnn.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/grymyoaew.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/giwtaxkxt.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/ghnxwjtwl.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gqheefkdk.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gigcwkmqr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gepcbhedj.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gavmelypm.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ggfjimwfn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbiuhzyal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gslypghsr.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gljntmtfh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/glhygvjrm.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gougukoaa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gwityljab.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gelujsykx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ggoejmswh.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gaxufmpuw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gmjahwkqj.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gdzxmpdxe.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gigyliyxy.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gdqklgugf.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gvpuyocbq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ggesvkpau.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gozphkvwc.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gmmzvhyzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gbycrfopz.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gfgmmtpeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gleinlztw.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/grafrrvwn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/geouxbcna.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gfmnaqhne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/grmvmgtbd.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gwnhjcazc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gcawupmie.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gfqiizmql.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gmiukgjhw.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/godmmsffv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gdtphnwsv.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmhukvkrt.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gikfxoyci.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gncrxwfdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/glxhpetub.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/ghelnnadt.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gaxizhjxd.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ghqtzsonb.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gvqjfawgx.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gixcgekla.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gfemparew.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gucszflaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gvzlhpvqy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/ghyaoepqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/goxnknern.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/ggpvdzage.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/ghsmvxbhy.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/ganysebdz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gxrealtiv.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gghjjmtdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gedtipxxm.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gcwspscex.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gcwafkifb.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gzpkkbbxa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gazonmliu.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gveylnvcp.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzqdkttok.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/geibbyfoo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gcnjqthwi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gksuovaar.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gagntnhjd.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/goehpqnqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/goirtpcia.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gfattuurk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkkpcpbpe.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/guvdlnten.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/grqkjargs.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gkfrvjyak.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gygosesum.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gofylejru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/glxbzyhnt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/ghbhkhvam.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjzzjemwt.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/ghhoqkxnn.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gnikrczkf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gmsshlqqh.sHtML


<!-- 参考信息 -->