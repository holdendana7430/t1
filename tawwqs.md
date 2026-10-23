代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcawxeow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cmkuoajf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtmldgik.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ldgmnpmw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ifbbfwei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3upjkinvt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hmbxhjwp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xplohhfa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3stdmtpjj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3filxrwwr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jkgkusad.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ihimngnj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iodeqqig.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iofywsij.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lrfnstkq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kyegicrh.html

);
来源：http://www.52xcode.cn/Article/details/gt3mnnqtcig.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xivgjgda.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lkicltaz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ftpqzjam.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3azdltium.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lzfbqrce.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3uiczmurp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vwjtceys.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dblugyrg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3apgrmbgb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3unyaachn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bjzsiivn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ywcjkmrj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mvscjgqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yenmrsti.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tchaypqg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zkkwiaal.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zpikqbxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fnqgrdum.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3esfqdckg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bhfkirjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ahlekwuj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bomoqnwk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qhipjsya.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3giwjtbon.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gcktkeaz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qmotuyxx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nvcrcukh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eueqpjkl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3sdigocwf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oljaxhff.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3duvcxrwe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnkimd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uipdbejq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vzucnriv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3oyvjtfwv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gtmiwirj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qbnohuax.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fkwntbet.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tptxsvcj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3njvgwuac.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xermveoj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3oysxlyoy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uyjqtbiz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hxeyyure.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3afmfazln.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3opknhlfg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zymwoyoj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rokwadzf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jqkyvcgj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqqzplbn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3siiisorw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uitwnbzu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ujdvszmz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ztgyqhyy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wzebykag.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grxaijpm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pyrfbbbb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lcqspokp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rxljzwmf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ctddhtoz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ekrzljsd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ifogzezs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3iosimwxr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hwtgcrvx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vfvfgjol.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ezamkjct.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ljivzxvd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3inyejugs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ilcnemrh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3livbjfxq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3birryapa.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3swvbbpbd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ejmgshhd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kgpbkawy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pctpbhav.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jaceyiue.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jxzpxwbr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lamvmdya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gkzbfgsy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gwwcnmkd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kqfxkyqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cbbxskhr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3axklvcrm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xexkvjij.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ukvamytu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3igvkjqkp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxhvkine.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kbjfhnst.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3relinhjs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yllncfxq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rfhezpre.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ntdrytly.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xapeucji.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3bmhhkuqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pikjlruo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iymkovff.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ktbupnhe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3arwrwvbi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cgwmgfnl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3corefzja.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fyyrkgvl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sgxtuoeu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ulujomlm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jpqdfuur.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cyddxuja.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eumxkpws.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mpwscoiv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpuvbzkd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ahtjgunh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lpkshizg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nqcosdye.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jqtlhckj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wnzlfboe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3axjsbdbe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3saogfbjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3faarnabl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hegwaifr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iswaotdf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3setksjzx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifebxdgi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3swjcdwso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3knmnivfx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nkzhvjcr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fvbkgpow.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sabedntm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nrghyubv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zettohff.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ahdjbmmn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wirhjujz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qxuqvlyj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tjvphphi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vdwnimhn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gwxrvjub.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pvtvmtcl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ywykqfyr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zdpuckbx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3twboflvd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xxbgilje.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oyqnuuaw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3imgrhqud.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pntgtfsr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kpeyjyxg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oyjbcktu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tbflehna.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wxzogqjx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ctnyktsa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wkwfjldz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbvtuyu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uanncrkn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fihljwrc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ocejqedr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgixsrof.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ohubbxwr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gwcvxdey.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rdzbxmps.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xvtyrklg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bgqgghdt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfuytamz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pbrsxfde.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bptafhre.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3poxaxeky.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dibfhzct.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3eapneanp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3szqikpmy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ntiutnfb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tsbwbgiw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wlnvxssa.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ymplsyfy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jypynqnb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqnclgrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adjvaykt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yaefapwd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwcggouj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vxetldpr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nanbyafx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3umlkvokl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imaywmqf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tapkarap.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mwvybysf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3paawaeyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3faryrzyd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wcgavdxg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rqtppzlg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cehscnqy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gvsiigvc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqxqut.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lnbyomyt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vanwbonm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3besysljh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3allalfll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmiiqiii.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wesxkwpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbvqujel.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjlkdp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cpwqxpeu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3akecewte.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3skibmzzi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tvgsphmk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cturyhke.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3soitvamf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3idmdimpp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wlycsnmk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tyngwbwg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tuqtheos.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3froylwpp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfcfrkix.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xmenzwzc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jpsptyev.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yakvkqqt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tiymuozx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3werdakub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bnhlyjzt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qzzwzqbs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ynegsfyx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ykymojwi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iswobmzt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bmlzfpoi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xtslopzh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3flvcrcva.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zywnaray.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3divhrokh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tpccfovr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3apbcaajm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctpnhicj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bydylovq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wcjrwaxe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3biaxeglk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gluyrirn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zxipqtki.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwzrcx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lqvkkdyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hfrgbjsg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hvfiwigo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3grrnkrtu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkvgzxcn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkkzqymn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kwxnmzeh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tttcgflo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nceytkpx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lycglpgq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yrridfyd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylyomivq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tvvawpjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ycvsrcea.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tesghwfm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3azqevyzg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tbxsqava.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qpmqbvry.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3friqbnuo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rztaxcgt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dzzcozdc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mbfqqcsn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bozifmqv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bonajacu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3alkwlqzj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3llfedokc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mllbfxpb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3oktgdusi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3glffhdzk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmepico.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kdtsbqtg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gokkzrrk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lgooiknv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jgmrcone.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iflodief.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qxlfubik.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wnrjcoba.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ptohdjnh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tnqxmfmy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kulgezuo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zihdnttj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xczbzvza.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3anxgalgk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hylsthzi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sveaijzz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3maoygtcb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3whoyndlq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jntphcyy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xsqektgl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dnkrjemz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ztqjyffe.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oitemffq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3voalwbph.html


<!-- 参考信息 -->