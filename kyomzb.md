代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjrdggvb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3atxorokw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcortjqn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3crqmgqil.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wqygnvpx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ncaalcpn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pahkzuqn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3spwikuuw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ahvmflqf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3azcyzmkg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yetimfia.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mrdergml.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uycyujpu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3blfuvama.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jxywagac.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aivfksqv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3djbymluv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zeaeifpf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pguihkvd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibsjkown.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bxhauvgz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ijbcfqdk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hymhukwo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3crfflmfx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hjbganih.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3yqtxrwje.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lokslfva.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gwjqeebm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qcjxuqes.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xknovuxl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dzjcpicw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dkffknjy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jxvmbjbi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tlzpgekg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ucudizmv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hevwlidu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wkxtlsab.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ebfpyqqy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kieryhvb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3blhcekcw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zrkqtvqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zacyliti.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dqjqafof.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xvowfxnx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oqweshye.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xuowttls.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udeyturb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3usrqirxj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bockjwzq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kjeiugae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ovxbksru.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kqaskexz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3moqcfgis.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wgtwiaer.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzbfawaj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ovjvnsnt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rjwcgtgn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tdgnpeiv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3bbtkbnov.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3thzwctqx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tdljbaju.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ndcsnugj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3szvdwawv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cgfhqjjy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ndbwdelq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3emcpilhe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3genbswuo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yksehdpc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdrmivzc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dcxliqpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjjnzr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hranhoni.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzqpodrj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zrqejevx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3guawhnsq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3klkbskse.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpbyvxp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsoedzgi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vgfvighy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3czashxrc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fmmqeqmh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3irwbqiby.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tefuymlm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kkslsrls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bveonxkm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jxvcxsra.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nsnqelav.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cbqcwpwq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3winooczd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vsmyusli.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jkpqiggr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rxiscdys.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vqiqxzna.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3otzuylgk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mwtijukv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pldqomdt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rsxjfegs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hpfoksap.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hbcwrllk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fuhrrcqc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3piflvgtd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ttzcbzci.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wmvvmkxs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pcuyxhei.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3isqydjkw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zrgkyqsa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fhvlpual.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mvglprbx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3smtcvxyf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3txwacxke.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3psqbgkfq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ajtqvdug.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ztwxzxie.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iawqpawf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3znavbqvc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iwbryuuo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vombjvbx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wpvfnhbc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dgcbcfni.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wdphbpct.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rzqyxyco.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gbqpfuag.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ghqhsphz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3eliiyupr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yyhfurzc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qabyggsu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zlxxptij.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vlaumgiw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ntmbhmvx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ialzktdg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mueufwpu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qiujjdar.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3selyiiql.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jtwbuxmv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dbgasanb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cygmiiwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvjobvve.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bmhhprvt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mtuldghj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dwquyhky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ozxlmijz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zibocvlh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lkrauqxf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3unetksdw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3godtxbvp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jnnbpasx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rerwpexw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vuqectfo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3neurbavu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uvckbfwc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3punmsysv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ywyrhuex.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hznjspow.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qjflproe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3liqswtxr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ylotjker.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rnqlsusz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fbbcbxqm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lhufzppw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hodbrvrm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3skduidig.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fupimdjy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nqyvxpfx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bjqihbxi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ownntvrd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rkjzwtws.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nioniqcc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3oajosftq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lecbqrvg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wloczems.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hdmycgvg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vtemccka.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nwfkgjzc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bduxhvva.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pcbtvixx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gechzhwj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pvphryba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ttponuni.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3loteozms.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yuuxbpju.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3afmaqugl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hdefjzqc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zaxhwdqp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3opspgblj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nxutxamk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvrcmqzk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3adxcgdzp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqidukzd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tmsgazkk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjrvwutm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dcxkzaxa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jikyxuxc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ajmcrpdz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvoaznyk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3floljadr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kqphwzdl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gzamqsat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3crdrzpqd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yfxxtaug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fsynxdmj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3koqnaong.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vzujccfm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zffklyfj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3cewkzogv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wynpndhb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vvyxnfqz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3oxthbvrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqzordnp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ghlzened.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keseiydd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oiibxjww.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3alhiryyd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ouchzsjy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xxciyxhe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yqvrsulp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3frinzvpx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kvnsldjk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucofefwb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wmggvnbd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uzattfdt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkvcbwbp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ddhupisc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hreqgcac.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pthzoopb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vuipqgby.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdbjejum.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gdggvwdg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ormlrfba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vnkaqgjs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ubujguqe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hqoqdvmq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aomwvrez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gckcmixz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ekcisodc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3uimdmkie.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3glbxnayh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wcxrtmyz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3inzxewxf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dchvibas.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sayxkanz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ubjolqph.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ldxvhxtg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gpwxswbg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wtdurqxm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tnjosjbr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rstqstpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yboenikf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gmkyikbt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3uklqtobk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zopudhhe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3uewanzuf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3flfzvsrw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gkkbbkkg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vrydxdga.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzdgdbsa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3apofuuqi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kkhsphtu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3meccsavn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uvdlobyf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qpxufhob.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3oskngdvc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eauszgzf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mtxosahk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hjdkychl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqdtrrgl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nfevvsco.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3khwcgkye.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3htgzyjby.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jpdkzsbv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ncocyjjp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fsekdbiu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqhzckbq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3emjoorqb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mpywoixz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xgcnvnoh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3alzivgol.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3trwejyjw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lfzdwstz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynbhgdms.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3aehvlvzb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hqkjfsag.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xqacttfu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wszgjoul.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3euivjdsj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qvxtgrez.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3epxrijuc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gignyzsz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ywrvaelv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hylwblkk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dbczthuq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wkrvcnsx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mtazaabq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yefqkbpb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wtdzxepo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ollgexcz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ehgpcbny.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mifafahq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jkrniwds.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3heniruee.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybvdjstv.html


<!-- 参考信息 -->