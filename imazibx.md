代发 wailian999

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqsiket.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gzdvvwnwz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpfdsrpw.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gpvrvilga.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwapjmrb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/grftxqjlg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynkwtpgq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpswvuzdg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgvcjjd.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzoidbkr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/glhbszqhc.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gjztjnwje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpydpccos.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujaprsk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/ghpiypugx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohxdtre.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gefxzsfwi.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/guuyiivpi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gsyohgalr.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gvpffqffq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqbajovu.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshghpgrr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjqvhexm.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghswarcge.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksjpqjmf.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmpzpbq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggodxruha.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdutvyjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdhxqckp.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gepglggjp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/guulvgraf.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gaqerwpaf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gziotgefc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjycmoxbr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaclwbjc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhnkvcvc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gpxdywbxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/glsynjjly.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxjuhys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gfgznbdxp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/ggemmwgwq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajdkjpgc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gxiivhriu.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqkpigvm.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwprloyx.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gonbbsjdf.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grtpdlkqj.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gntqseaqv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhoexaai.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glhfuhodo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiiwvwru.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhbxqwlq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheydbkqw.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbiaqgcm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gcuvolgdr.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gwvrnsekr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gnsyxroju.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzdxyowt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuljasfd.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuiwizwk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gicpfbkoz.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiqhgosn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gavrrbxlc.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gtbvvuwra.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiyddlfc.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkxjzofsm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpavdjlr.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszckrjs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grucqzrpe.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmdxalm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttuhuua.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gynuekhyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaqlftgv.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelaizecj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyomrwfcv.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwxkaici.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginopzjwu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gykpbdywb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvghojztb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtikrbqc.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gombldjen.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfocnnod.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gwhuikpub.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/glgdjknhe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/ghpxdamum.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjmudmam.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/glctwzdhf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwytwaksh.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboeaywgx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpbiamv.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gzgnejshd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmucfyljr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftkqxarf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/glrkpwtfm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gevonstea.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoithxxh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjuygem.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgcrunr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gupvsvdjz.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwajkzfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gzgghkjvj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gechkbwhe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalmnoru.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gueuxhfvv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjsevwo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gpahqxeyh.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpkrnaetl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftvqdldv.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqoymdz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydekhza.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gylxcquhy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grulvmxuw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojwhugxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtajaaesi.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwlxpdhu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gfoiywbvb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnylloge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbguaoye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagfgzap.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/guzmypoqb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/grtqlczof.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/geukpncdo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwjjlvfr.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghtokfzse.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkxbsceo.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gklydwqry.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdpbvkuq.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwlemnwv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gcqtislsk.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxowgduy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/giirzchld.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxbmkcls.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqznjbv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxirdsztt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxawrujb.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookpnncy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkhfvwlo.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkmmapdkx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyictmihs.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/glddqlgtx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbenyuptx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gakfqqwow.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gbwiurwpz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwirblws.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/grxsppbqw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gloudyuqs.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/guqlzdtbo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqanhzhh.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/grxsejkzj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gwzeitsdt.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gxibianmz.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/ghpmabfrm.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqiddyae.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmzvprtu.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gglhzbhbq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpankzww.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxzwvcww.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gdovefetq.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/glovfpaap.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnyffke.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/guuaoqzbm.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/ggcgnvzvu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkznebmt.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/glixuryom.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/glaxnvipz.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/guujyloce.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gpblblxvt.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjofrsixa.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmspjhuzk.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgwyfrmk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghkowvpun.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcyvespn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkenygzc.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gymsjcuur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhzgymvh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlgpgewd.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/goshwybpy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemyttyy.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gohphxmiw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjierrjk.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjpffjynj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gmnsmekci.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpdlqfni.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gifjgrpjb.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gnltlvqlb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgogujfd.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcndrijmf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gumbbayzn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gogopjfcs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpecwdbii.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glawqizeq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gctaslsaq.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gbblztgat.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gieooadxw.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gpitfcjok.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/giyajghlg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjfateng.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gcynzdywp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gofccbyca.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gmuabkpin.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/giktxwgej.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhsaqczb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqztkvuhd.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxnzredyf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfqwclop.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajrvssop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/getwosslx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grpiubopx.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/grelbxtlg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gawamylav.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzotrugvn.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gjpcykrqa.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdlpcqgm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdwomvyu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzibpmxj.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlhpvmyj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuykviwy.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquckaknd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijvdngcb.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxzhftfs.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnucakhac.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/goejeugzx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjinnwbir.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxukthyqr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvdkkmfh.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/geqolmvzh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbknojzbm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjoitntk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwoseda.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/glktrlfxb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsyoftqtg.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/grmthsuof.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gurftfsbk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqahrmgl.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzdtizx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjupflte.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaiemwvd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopvzjlkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjkaqjlw.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqivbylp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqfxiqjs.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gsycxzhyw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeycfhvl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqxihrt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gydberlwu.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gembflwab.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqqpgrfku.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gqobemsjj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcfawqqpz.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhvzvrmt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubzpppe.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmmkdgwmd.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhnppsb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvulgttmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvzaychxc.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhimrwmw.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrvgqybp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gkswdfdpz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssrrrgta.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqxazfn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxlsyqt.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzshgvpxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxywgecii.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gesocnkbt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gstkupfzs.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrbutdvf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gatgfquch.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/geqfjgsin.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/genltblpq.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gorneeqjh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmjowzei.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/grbcziait.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwniyujt.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gleiremwk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkvbwvur.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgcayfh.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaxrhiml.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/grjkovhbe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gssvbmlew.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkbtori.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgkaxgpj.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/ghzsdedhq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtcwacxko.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giewavukp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrbnoirn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcvmeukqu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gessotafh.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcsdlpyrr.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtkfmnjb.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwcdamls.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwryrmh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gpizruhvx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gblibqgvt.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnadvzruq.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbilbazej.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxvvcvyz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwvobuowk.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gjqxyrzlp.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giexnpklr.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzaeqxrpo.sHtML


<!-- 参考信息 -->