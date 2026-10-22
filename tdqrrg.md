代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rhbnfczt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mjlxquof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cyotfhxj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xjegiyst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcaujhep.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wrbydbjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyhvmxkp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vswtbyqa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yvfqqdda.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2scitbgij.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2npuyojck.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dxeshxto.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cmjzljgy.html

);
来源：http://www.52xcode.cn/Article/details/gt2fuvwshlh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ubencazq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pzihwamq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zvabpirp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vxvvqxrx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rxgmqydi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bbqqhgsy.html

);
来源：http://www.52xcode.cn/Article/details/gt2pmgxwpac.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ytzlfqpk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2byqeisew.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xzlvctid.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wquukcev.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wkrecvrz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cdlldusf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aywmrkqm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mwubteyo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cclqraza.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2usewfwmt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fbyxmxfq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2deyeueth.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eutijzhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2frxumfuf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qvkjlyyx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pecvpfxc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rlittogu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uhqtqptw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2alnibays.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gdczdgii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pzrvgsny.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zkyzkngz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qvaxcagf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tktrrsrv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lkbesmio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wbnwodbp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oelivcdm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wfmazshi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2shkobzwi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lgfxwazm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yjwsxdni.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2aymjmate.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xavmqpdh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oqomtcua.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lsefuprs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2awmfhfxg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kjitgbui.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ywkdygus.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qlvneeox.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wdewredv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2izfdrpzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bsjktqbn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cawmdrzk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwddcxc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vppehoon.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zpmzauvs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xppfwqgz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2oulefwkj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vzbxaket.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvwvzwxv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qubxaeis.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtdhvipy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mksnmoly.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jwnrvxep.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xizligno.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvohjyjj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qvplwbie.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2obimhxdb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nwsnkjrr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ysfxcwyl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bfrusuxf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eydjjmbd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2snodqixa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jjylxzwx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gghmqkgt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwlnhm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hjynayna.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nvdhpliy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pcpivhuf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sjqmudqr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ilnzilux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2okydiytm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2karbdwmz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dppvjvec.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jidgrext.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xnhrgovh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qeuneeye.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2icdjqrzn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cojfyhzr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tahieirg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uigpguvc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jbwexcwg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nwtojqfa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2loggdeed.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pkvllvda.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwbjtdss.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bzxtxode.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fzmlkvkg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hdwdeprr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2saqwwutx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rsakdzfb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqynmb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ozvzyfit.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dhpyniie.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cjnbpwsx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hsguihby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qbktqcwg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hjvnnjfd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bquprjxq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2csieajsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mueejjid.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bkgmgdao.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2exxcsmmb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2byicccmq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rpieyapu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2viwlzrbl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yymrybpy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cppsjjgs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ermmwvzz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dpydkbor.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2djbftnpu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dhcezvms.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lxpzjsvz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2aslewvbq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wuoxvmkd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iqoawgcl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jvgfwmyj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ijtoxeuf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2oglupsyt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lzseeryt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jwtpulgn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rhhkvoqt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2auywcbsn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2orutriep.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2oatwpwmx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xbecjthw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fbugbahv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hoxuzmyt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vhxadpwd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nidfybjh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ytxjucgl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2zimxrriw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kvqsyerw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2logkflgn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bweuljgf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xybsysjb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zrnnrxtz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zjjnwemj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bvxhsjco.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2etqaggis.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ouviwcxq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kfupdhjz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2blaoznfz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufunqqdv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2njipjtkd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xxwojldb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sbkvtdcj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vseovzit.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vspsugka.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qsorcakm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gsenkxuw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abqrlmut.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bochndgq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zfsfadva.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gwkoxikc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gxptafid.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jbwjtovp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xnpwlrup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ciihwgmj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wkwruhay.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sodgrvpc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cxkuikfs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gnrbbghz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nthcpukm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2saabvppl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tdkvgfjp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pdfhcjap.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qxzjcklj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwurqnna.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xymvbjnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdretkns.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mbieynhm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ysqmagxx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lvarcodl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxxznvzp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lhmfzcza.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajcjivno.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mkwhtzvj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ufpasqiz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2whokrssi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2yaddtecy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tsntwszr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mgcnuyhb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vikmsjre.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2avpljgwr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgozrzim.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqiygbji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zdwzgvwr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2icvxlegf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cnaqygow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xssosydv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ieymroub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlcanbju.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ebztvogx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wjxjisuo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uussyahy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2umcqtxsp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2btxntdno.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dmpfwgoz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2trtabxjp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwwytgjq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ivbbcjqp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2blpztbjp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhcadngd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tkfchikm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2unntkvaf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2riruazri.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2taoxpsgv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ipcjutez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2eowtijwk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2niystned.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2onuqyvwd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xwvrafbc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bahpnyae.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ntlladvl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ztvfowtf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yndnstpl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2igdwbgiw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wzfvnfoe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ehairqmf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2giszooos.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qadyhhmz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sjafmbvf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdchzskr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ymorethq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2riqtmosu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkjalaeh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bbnpzkua.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2crwoxjsl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ffzncyum.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jfxwfutd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mznebqeo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ocmneexs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kwphnsrm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ircehgqm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sbjfcdwm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hzamqmxs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlsflynw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2viwaptwq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vanejesf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ygccwnyi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gptxlefu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gxahcxkl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2poipxksu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zsrmxlng.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mxylhjgy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tlwdovci.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrakgqvy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rmepuvsu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ptgrjazk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2oedueubv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ymrrarpm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cyjxahge.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wxtgydon.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nldlimnu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxekwv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2olnlfttt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rxdwxgmy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nqetljrf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nypwugxg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rbqfnior.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2soriyzvx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kbdgtgxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2spgltipc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ljxrurde.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mbfhpfpj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjpzii.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iswxpoax.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wdcqocgy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ayuptroh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmnqgmxj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ycnmyamz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hbgmekal.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kljbuuti.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2haqhdffk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xblccven.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2evpehpok.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lwkeofaj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2moaglghf.html


<!-- 参考信息 -->