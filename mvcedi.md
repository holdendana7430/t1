代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmmwusak.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hvjegngu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcbljxxl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nnbmphqp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tijvmrvi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vbxrnogg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jhwmtpcr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qvaeemkf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yteeaivj.html

);
来源：http://www.52xcode.cn/Article/details/gt2oskotefz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cqynjxyw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2qxzkbwgd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kisknozo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2msrtessw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yswnaegc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hvibybde.html

);
来源：http://www.52xcode.cn/Article/details/gt2mljyvnwu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qscfqkjg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ezpnwpsz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2susqrujt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jrjerfwc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cvlqtyqu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2drjxzywe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kekflsov.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2swlhvbsg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2upoxgekf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwxkqcod.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wlpdpkuc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pbrufhst.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wbhbvhtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qkwulwku.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xplkskdd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jgqsmogk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cdnswrcz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2krwaidcf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lfbhdqfx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2glxwczym.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lndjchys.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rrfdpovm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lpyklyvd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ygekparb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rwpegvls.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2cwlbodnx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dycylgcr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czsbqopo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2doxyusmu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thwsmayt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vderwlsh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dkjhnpdo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xvevtfvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xilwyxtz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lfolqdbf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2scdgiayx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tucklwbf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gbtdwehy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fwpffeit.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sflnksql.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nekanbsn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2scqjubxs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rgwqomve.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wyqisgab.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gqwzqyjq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2angntrye.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tsahljau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cvbkvgnb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2svqffrrw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opvbvkxq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dckbppmu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rshvoyqx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jotderln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2klvfszbg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ybnftwqn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqjtlhts.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2amskfmgj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2knyjfmay.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ygvfwmzl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ykuerctz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pkldevte.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xpzunyww.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ayicsmkj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wcygdibe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zgxbxtea.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2luqneqrd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fftlxuec.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2khoxlilg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtgfgupm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vvpyvqcb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cbmydipp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qyahgnpg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2scynbhlr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jgwrgtpi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bumiunxh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qkxrwuot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pwbuqknn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zjvlqyvl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rebewakd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xjkliexy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jvadwtuy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bkrwpdec.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hgzfnvrb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gxevylbz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2abhmhdwz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vcgaxhhz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sktmvgeq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ynlfjava.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2craglkoe.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2inesuqdb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rnthaxic.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xocjafyp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mgkhfnhz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jtuuzqda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ifvsmdba.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ykimefzd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cbzsmckj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bqdxyhvo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pjjzdphx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wohqeqdz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ngjtgbma.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2knsjnxrw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yoissrwe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ktyejrea.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jbacyczk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hkqymsda.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hnszxilm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2chivycdj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bozwzpde.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ztszwgfe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2twnzsiis.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wypgjnvh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hglzuutd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eyxwebhx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2llyeafqi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zjaflbeg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hvhozmmy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2luiqldqa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dbyqzlwa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zsraaeme.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ubgbpbmv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vysrsyef.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qethqjxv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yafvczam.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kunynlis.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dvzlhxbu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jvlfoyyh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rvnpwjof.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzydbjag.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yfslpqih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2afpxdmzn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lemyoehz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qxkufsxt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ueqqpken.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2btqptnzy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rgwnvgon.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kyquzaxs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dejyquva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2znkcwiqd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dcyrixsl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rfntbvut.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vpzopcbr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xsjyxkiv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fjpbuymm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jgadawmy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gwkshyoi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wcztnaii.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uszkblxu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2svqaqxfz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2skdurwqg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fzsclvyt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvvscrmi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ufsjfdca.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dfejmfwb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gbreexje.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2itxayzgm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kvgvyqcv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dsukfxgb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xrmltcjx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yjmjjcif.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gzdjbfly.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qihwpuyu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qfujbhop.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2crcjxqqv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zywtywsl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rcbrefjd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2scmzoxjc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nvpkcmpw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkuhofeb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mjqqcjwh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfjemfvo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ocnarqnt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkrfizyp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2quateohm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hdhfldyo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jjccuiye.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbyvvluf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fpuelhgn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vyjazrgq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ojelqwcr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hoijdzcm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ayoexvyk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2juyztukg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ivqckgjo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lcwghtkw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kaaivqzj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2agchjsqg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hknfajnn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cswujcnz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2khiauqmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gartiomf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rewzwlui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqqgpali.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qflntekx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2iqxtgtud.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zgnamfkv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nanufais.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2sqabpzbe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mhdrisei.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qoginoyv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nvcaayxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2btjxstel.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2acxlmujl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qzzskmck.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bdplreqn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2okkvbjmz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2byjvotiv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2derrrwqi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ivrvspzb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2eisxgmxr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ddmswdwj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cfkyxvjh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gevbwzgo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ewsqjkas.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2akafmdkt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bwjunrzr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dkvyfydq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wqgjruxc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fqtqwryp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lcotpngl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrhybrkt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2guqzwucz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fdqffzsl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vpjlnccg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2flvipzqs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2szeqjkxl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2utpgmwka.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhlyyxut.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ovqkeoxz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tqyccgso.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vuwtgelj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2kpbflikf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yzrqlagt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zwjsqobw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qgsbfvex.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ydtvmvva.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uuotacaf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wexogrtl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2epsojavw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgdikmxv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zebpiekf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2khzdmnxe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gogmyfcu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kterdsjb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hdlerqch.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bnkjoqva.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vupwzfhr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhmgpkps.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2agfimcxa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2htapiebz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xsyybicn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kgaeqlai.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2msimkrmn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ljkrbvce.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2udlelgef.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wvtsnbow.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2benwxzeu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xtcfqddu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2crodcerd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zkydebvx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2stuctjik.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhemfknv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mqoeduxb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pnrajtms.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bcxnwlru.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nazvsmib.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jnonoijh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hyrewelk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cuhvxyxq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dhcxlfti.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvqsbhzx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lqoqjuza.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pakbhsvg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ynyaywfe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jycmgqnv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wiefifeo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cftpbvss.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qqakackz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vnokasee.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eaxlmtzq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fohanbvv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cvsxaiih.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2aoomqqql.html


<!-- 参考信息 -->