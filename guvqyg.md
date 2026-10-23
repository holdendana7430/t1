代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvhbwipp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ejqlsqvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqaanbox.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qozlshlr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wkunqcpv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ughfknzt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dgynmblh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3szjxioma.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oclmbysx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3obmevbmb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wnnpkdbe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3keoamqjg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zdehxumk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3garsbiuu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zlthacml.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjddzyu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rjixghrn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dhotzthh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ebmbhfyu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sexpltdr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gkabvwuk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ksctmoss.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3keolcyha.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pnhophcs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ptuehzvz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ubaxhsvq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3nohhlzuh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fhfnhbul.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xuilyaqj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sloqfhui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ixzyigaj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lhscvsrp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3prvnzagn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3iuovgetw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3duzgbsmm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3athzbcon.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wsxvofmi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qnmbpqns.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wxhxwaqu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lxhathfo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qyznbieo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cvlvdbrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zwmkaffw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eijoerce.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lqysacgh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zbqhinkm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utyfarco.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pnxftllp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dridgqmv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3utqgtuaf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kwcrtmth.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3chmdmswt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3omgapdsk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cyzrtzof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nyuvhbdh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vgcwziqb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cbrvleuj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nnnvtyuh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wbrwlnkr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jsrnigdd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ahuxatjp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wdllzvpt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dcqnuhop.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3waaessmm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xpfunyjd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rudckwgi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okankopk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vxkavbrq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lonufbkd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ecwjipid.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vguothpc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gclttsje.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gouujatc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hhcswbaa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3smhzrcjs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3njvajfhv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nlzrjdnp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jesxaodz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kcwpvzfk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ohzimaur.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mtzjbbtz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wyahbsfm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xvizrydd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3idqrshoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ymzdrhns.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wqpfmxvb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mcbkzbui.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3izqkqwux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3likzlond.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aubupcgd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wwcxtdqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3iqxcdyec.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ftfpphdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3comklwog.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xykfovon.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qgfdgxkb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtgjkl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oenyaqqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3cboftgsw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bhhlmedj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3binjqryc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xsrgadkw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3efnmezgo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bqvyrxpc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3thrtnbye.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3whrmyijr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tlihmpuw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zbvgfjvz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3onevqxsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ustrawcj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3icxssfyi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cuvbcykd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wcaslvbp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3exvccnzo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rwhfxspe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qmocojio.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ppbpkrpd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhjzgvh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3akpseysu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ngwhenmd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3refmfztg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hrepwyrk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jiybgeix.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ikzmvddn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vpfrrygx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hkkywzpz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3apnqrbao.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cmxjicwz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sechnjsh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3msauylkv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zivpnkfk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rbijwhbn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zeglmiwv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mpjdlncx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gygbwvlt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wfrlokkq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ibkyaojf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kcgogbaz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xmpijnbq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3eftwibdx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dynvgucc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mwwsziqv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3puwjeywh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pmzjukuw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xhnwiuyx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kklcayiv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3esgstsuc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qnwcjzwc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xyopwrza.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3onwtpsuy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xuuvnlgq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hdfbawuk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3otcbczao.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ukqzjetr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hmimimvq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tdiafxat.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mqndysgm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qidmlklx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lneegoli.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pqxlfavq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yuhylhyu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hcxqanpf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rwabyxjk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cutqekcp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzdcmczd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tgkaevwe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fhrmdsni.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3szteqvtd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzrqqhmu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3aaulxmum.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ucnozqou.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dfbhgzlq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hugxxwie.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lejuqbnl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ffthurjk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3eyyegaer.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xnpeyogp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fzvsmwmh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3oselklyv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xgvngxjw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dcihzsmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3snhjueuf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ixbxqpov.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tmormfrb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ajkpfhdq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huvukacu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3diwderwa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aieyfjio.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pxumdmfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdawuszl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yocwimpi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mseiidtx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ukbepcxu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wuffkfti.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3scsvwkls.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tvrstiob.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ypfgtjzw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3khquwylu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wmsazugk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3caxuhtzx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yqczefdz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kojdcdsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dnvovwrl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rkkzqkhi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vubfmdpz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pejvynhz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nbqqxljk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bevyagcd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mblgjkec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfujcktc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3biyxdkdt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tvcbcesp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lugrrpxx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vtjdmlbn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ypgdizhh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ayoifyqg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cqraviwk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3owbuovxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ijtpqpxl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3orbgkckx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypofzjvx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pecmvsbl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3emhqnzee.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqqgwmgp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3irgizquu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqqshdhn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xvhdkhbz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fsdikzjh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hteueovy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eyaknpgj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ddlsnnjs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rsqvqsfz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cntwcirg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ymfinltz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3enboscih.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rmxqqhhw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hbkorrkv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3egeceptk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yajqhden.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nyeesjsy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hdmqmxin.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3crbowgsy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3abacrajq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jftkmdio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zwqbarcp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yyutwrmn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfwwjqqj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hvbcbcmk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3spybgycr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ctvbxurt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tbccokyo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmmqsvec.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3afzaxyug.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gsudxojv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwlgvvvm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3grxduadi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wfaobjjj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cpoelupq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddkgvmwa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rtvrgpjw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmbbbegu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nzmfzonr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3swjgfvil.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rhdczqkf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zrbdwqnn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fsasybxt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3omvfmkkh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hjjasslg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kepkgzbx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bjwplbhf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ptaoamdz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpjmifxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lqedkfow.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rsrtogwl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cgrqeatf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjokyndi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psvyfptm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nadqcqxz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wwdeoypw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uaydwfbg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3njdvvdvz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qrofrpgk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rzsycrgk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3circcxvx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pwmxwwns.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nowfstva.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3llrsjmfu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3aeuzxihb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3irgduhmd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ydkfboqx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ksxitten.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ntjiblja.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rxgcscub.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rcshiupo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hvesdhws.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ugqbhrsz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tnlqzraj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zxfkbgio.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cpkyxnmh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fjrlhbwr.html


<!-- 参考信息 -->