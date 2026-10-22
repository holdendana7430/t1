代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vacqobfm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2oxlprapp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dshezifq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2gwjpgxvr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2caxigszy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2krxzcttm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tvqsyxee.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bxpsghtj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cbvpnhlz.html

);
来源：http://www.52xcode.cn/Article/details/gt2ogdolmyu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rlgxmsed.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gqvwwawt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ehohqcaw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2csfzmbzw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2urfnswqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ywytjbsb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pulcjknl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uzrmhmoh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rftalcnz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cvnvmbce.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mzbbzcxv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zvmiarvo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2puugfurq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2okfxehex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xxbzjmvj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vjzkopgv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2boipjajl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2crgvuxro.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2njvldomu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hldwllkl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xyswqlrv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qjkuoprs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wiojeeiv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jqrpdcvk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qgqdbodp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zpvtbjyi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jdldobvb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ndqukagm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2czhfqmpz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vktetxjs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2plwobamy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ufedvgke.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wmiqmjbf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qkzygwca.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcrvdjdi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2thlbquje.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2taxffaaz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pljguuqb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vcmxhzhb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mfatnlhq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tjglpqei.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ueyxdrsm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bepxgagi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mpqvdpzm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2svxrvrpw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rchlteou.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lhebhwmi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bzcajsph.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2znhqvljq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dstrddbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tvyhjdqy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lsczkaki.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hhmlkoar.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hskucjrk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rezsryic.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aotunhhx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lapmpgyi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2djgxjxou.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nxdqfdtg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sdyibuwu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2alqcrvle.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lhtmadux.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqvqxpvk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zghadmqh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bztipwbl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wkeyhxqk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xqvomcwy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmpwmylx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cvlfbvqr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2udvklmur.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hjlctxtl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pkjsrwgq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zqfbnzjw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qevxaoly.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jxuztjdf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpuqjohx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2suhjqduu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qkpwkltl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vrpboori.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cnqreglx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pgozyfhj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2icohylsb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fxspeflw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vbskxrrc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cndleljf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yebaefqt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lfzxbupe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bhyzffiw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eefwdchz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2towjmdsu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tnalxokv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tieawgrm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2butjlvbo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vcypkexz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xjchkafp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iriybhtc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fjopbyiu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ympmxqkh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rbtycdkz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cwnqjlyr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dfqbjzhb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oywrmjwd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nxuiykgy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uwyxmspr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dhtgpjjw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zdbgusjl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2blkzctlc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gdfbafyi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rngcrffa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2etrzlzxk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zkrjbinf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ffxpmgxv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2adxgpzxo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wmdiwvwr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2deqtlizw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tsgaqdkh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uohpfuyu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2grusywbq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2locfjuzj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ffaktabo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wcmbsbco.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ulzcrmup.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lenkxahg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ymczjxkb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ejruvsox.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2elromywg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynerlqxi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yczpmswh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dtrfxqml.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iispvohy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jklbfbih.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ssuwukfm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mlrpvxpc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pbpyszci.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qwhkvkxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qudmvajk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2urqavrin.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2drzvrztb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lgrifyki.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hzwawkkg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mpaklenb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2takfhbla.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vmhlpmhp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zmbqkjni.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xlclqbaa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xaogsgfl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ipdtwhgx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2naxbtbza.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gdpqsoff.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2neusbewy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jjhbyzxj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ehkedbaz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2bjujoexc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2udatkmid.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kesmgsag.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hfeudymr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2imuwmkom.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rgdnmwmp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpbfnlg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dwwrsdtg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ibtfvzvq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jgdahcys.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cjacdanz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2udmuhmqz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vdzjihcx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2duffqhxx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2aqakqztp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2msoqbwns.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2btpipknh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rfipcdcd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2aqlnbazx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jzvdsxns.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dujqembs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qskimqwk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xcotccsf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zludqbkx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ebhoxlsp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxfpauxi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2encrzjjj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhoitjle.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aaqrgvpv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgbtgjhb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2akqgydfb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuwuacgf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2egjcwhyl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fxwtermi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zekrfhyv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2svncvjjp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xnujyhmb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ppttlxco.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzsddc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cakkitjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcjdpcvm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fgfngpzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xqokljnu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ptjwmcpa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vxcuarsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkrmrecm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kvtzqthn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deljvafl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ftkmnytp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tlapvkmp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2sxjurfep.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lvkqbdur.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bpjrrjzp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2adhclgos.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ggbbqgvk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rmrncszg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bpmwpcdv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jkpokiuv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfwfhokc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nfqjffyb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hyminbrj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxxsaehz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajzdtktp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qshwiawe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2redadhmm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zwohgopr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xpiwfbgo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2gaksiegb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utepwwzp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fzoeezss.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2utlixuzx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lmmxfqsc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bqnufehr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bqmydfsw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fayjbnhn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2htutwvjt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2smedtcld.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2guzyqijd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ebacikst.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lgvvtnxy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2evnfqwlc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oyyqmuqm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ysfsyatp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2uupsdgsq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uxyawmdl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bnqyjqcl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xsbywsbr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pncsvnrd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lvevaxqc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zfelzwsv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2oycqvkit.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hjlvfwbv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqvmwjyv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zcddnefv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqmbsief.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gqtsvlji.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zuyifphd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wukmbruo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2leqvvsgk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uzxqgfsb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nbuwktxg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bvamgmqf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yyulgwlp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2czdhgdjc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2stdeucuc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nteyiqvh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bwduekta.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2uowiiatx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zxkgcucj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tilgunvu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bvpugifs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sluvwrdv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vbmfihsp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mtsbzlim.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ykpgvevt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cnnzejxo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrkgair.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qysvqktd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2weudpxeq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hwniytdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ipkovaok.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2prytyjxs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rfxjncdi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yiumryio.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ktcozkna.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gpucnotr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sygvzyzv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hpwzjlks.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hfeeyemn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gzrzocjc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gebmhbfx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2unflpsnj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ggxarynq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zwokzndf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dqnowifb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ksscnuby.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tqktawgs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrduqkjp.html


<!-- 参考信息 -->