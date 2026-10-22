代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2znfksnnj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hydndkvi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2flaufguf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vjhddkce.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ltovrnjf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fkpkuakk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wiaezvgc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2etlcopin.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fvrerwxu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fedspydg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qqwylngv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jzygmdqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnecdqje.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dxamyjli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktymdvku.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cfywsyfr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2atimdtez.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dinmomwr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgywfm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2trzfxcdj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pswlczlo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jclfodib.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aagqfemi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hqklmsdb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cqahnhnz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eszjdrcz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2merrsopr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfbtmha.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vwivgnrl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ktxisisi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xkggkdob.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2icoztqhm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qkwpctya.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2eqpxislz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2czpicjcq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qtbtcxio.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hhnldxmx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vleytbcz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2apoaonkj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mdeaaxth.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ehczdovf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zyvkwrvs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2frvqrcbx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jrhjqmml.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lbxeorqg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2viyrhugu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ujjjarje.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2aqiznfkl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ezzabpgo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lirbbnsv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tfzgnhuy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2slefkhda.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vukhdwsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kcgoankd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fnvvqtqg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bggrxoiy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnbxltzs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2oodkktmz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tyfuwhxz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xoiktlqd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrwawg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jyqyaizb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vjlhrjjd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hrhzgcpx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xmikewlb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gkniutbn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2taysvhgk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gwrwhzhr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dhukvrag.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mhnvjevv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2gvxmovzi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ibuuitum.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sdfvjdit.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gslafysw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhygbhbt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hfepmzyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qchztmjq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2knvgzzfs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2folbnovg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sptrjnoc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuvczfgi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jzqzjcbf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tbvjkjcm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2boftzupz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brvcwpss.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2croordtd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2geupqixv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2utfulvbu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2winihsks.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrnyaoxc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2edibeapn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ecoiuyty.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xfigypjp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ifqizogz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2yfmugumi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hwkykhql.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ovwbnair.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2azwotvwk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nvlxgeaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gertsrtt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bmpbjdzq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zkjzjisl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2whcexyrn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nwanaomx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ugllhzof.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qtxhdrli.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vtwpsral.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bgmmukpx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hbdgngek.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2anptvubq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mocgqdtk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vpreirwl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wrsfjlfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zjpsrabt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lhydzexb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2neaoxwxd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gqqywwvv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lhouxikl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cgpvcpdo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2aqgcgvpu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lztwowdg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xokgphyg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cemqkthf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2odlppejk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lctytouj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzeojzi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdtplglk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ijixshuk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dvlfkyht.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2phbrylpe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bdtsletc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2sptuzjoj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sylhmvcs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eexfxvys.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dzzxlswl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rejjkmks.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2nykoqjog.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fynjwopy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aceixslt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2opungvrq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nemwfpgv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mciuxjxv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2cqxgplbi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qrzhafri.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pmxloghl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kxqtzfif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jldbrmdw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bssbpook.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obvfrovk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gqekfpck.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkimrzpi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2znhpnndd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zcpwxeaf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kxxfdvha.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hmuarnus.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywvpsfgr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2aoahckad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2esygevkw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2srlliemi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ldrygwap.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2uzjxzgqq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2purvqdxg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2opuyqjia.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gkkiispe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ysteyowh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ohxzwvid.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2euamgova.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bngowraz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ywhwuoul.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qlayzanw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pnubqlxy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtdkacim.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ycselquh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kfyxqkgl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wlpedwuv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bdyghzah.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsnilvec.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fptmhqco.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2czllvnjq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wqshfuhk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2btbubfbv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ujroepsy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2svggpsrj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kxdcwcrq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2txuerjpp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2faiwltfi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jfvafcee.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cikarjhx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nizxhdnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mxirjzfy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2upocbtml.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2eyerytjr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wrwcgxcs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2weendqxt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gqpwhist.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ugxsaiim.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dywoufna.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mokhxbzb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2redxqppv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nldazszo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wynumbww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpzhlrls.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgkzcixk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhixixnz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ybgdpcnj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mytyyoao.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ihvgcmfc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2frmymmgl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uareqszv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jyuhzqpu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2olfmoesp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2eckkhwxa.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2drrrbygn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gighyggt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfwizphl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dtowhwis.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2onyibpyw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zrjhtnku.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nxqzwvmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlblosxh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dhsuhfcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkuttxng.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xgnxstto.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dluclyqg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2aibrtguz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gzjhxvhc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cobfvrwi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dujepssx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xqkejhfg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gikkfhwv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ztqlzlii.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yargafzn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2biztapyj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndbjkkxh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiuksgln.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nydxnrhl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yyhdkygf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lbjqqruw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tpeqmged.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2umrmtapd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ptdcqobt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wwlsgbvk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ozobowqw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2txekwtsg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ctongmwc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pidwdcas.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nglxxdhc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kysdmxhx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rzhzxpdl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wxcpkebx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sthwdcjk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfjrjxha.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwxeszjz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jijutmuu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qpwsjhrv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyewcmep.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zpmqxsqr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2czbapkqx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bqukpyvb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sxbdsuzl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ucdrozzc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oycborec.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cgqfzwro.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2grinfbbg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqjgytri.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qstggrjw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjgojrbs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjphqtaa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ttlzdzgk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qewvgwsd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gozxxqaz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lmsevcwp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bzkrwbik.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pyelpezo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tqepricp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ynehrguc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2haloqqii.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pwefhjmv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ydkzxktz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aylyxvma.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pjezfftt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zsezcjnz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fydxcbxg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qukpuwti.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2sqgpcfty.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lxntcrdd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xokkqrpz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2npzghzbu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fwwtgyum.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kodiknlj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xzyjcjhx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mgagwthp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hjwyhqvt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xiqlgsje.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rjyszzjt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dmfoqmiz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2brejnzfs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yfmfsjtb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ypugcoax.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2atyqaltm.html


<!-- 参考信息 -->