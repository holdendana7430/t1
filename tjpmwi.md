代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xmttqcbc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ygqqzkto.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vfwhotgu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bmwyvycr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syoouyag.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dgisdebc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awngocbg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ozkmjguk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rkototuy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lkbrbcnw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wlduzxzi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lbgdcdrr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dwabumrb.html

);
来源：http://www.52xcode.cn/Article/details/gt2megfsnuh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2sgutywdt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qgxklhaw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wmkspnnz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bzlhgiup.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ywhglnfd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2epzeuiiu.html

);
来源：http://www.52xcode.cn/Article/details/gt2bbhywthe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2irptamrw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xwetxeyj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfcrfnez.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnflet.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tngetrss.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kqhteodw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2zzufstyg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2azvkplwe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wpnoggdc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kuwkzsol.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2erksizwf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vozqanqc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ngqgsruw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ivgirzvf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pzbcklsh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eeljzzzr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fyahofjb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2scgtlozy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2penwuniv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2duoexnkx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pqkauhnj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bdyofkfi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hsujvvxf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xtlrkxgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pfmawpvt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2iflazwou.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wmlgmmxx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nczwryij.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2svtmzcng.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqmcvos.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xvprtytf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2iufsdjlc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oetsfimj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ixckxuah.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fsueitim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mkkreamn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nvavyvsp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2txgevlol.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vakpnahf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2djemaens.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mtmgpljq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ayytesge.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dhqikjmq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2huphimnr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wybbfndu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruhciged.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ipzodref.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qxxriyba.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hkukffyd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2infziulu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ydgtqjpo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2odofqmkb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rlnuadek.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zziojunx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lhfhzjlw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rbyymbnb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nhvobteh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oypzdcdy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wfovtzrr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yxpvlvxb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zafkaehe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ocmrvvcf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dyujuerw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2szxfhleu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bswuugsx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2usdaugmc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2eqenhlix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zbkazzgh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gurbnfur.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2csbqfjpt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zriihrhv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2oivqrjkn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lvnwfhvl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tahkahiy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dprlrxte.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ogjuohvs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qpkscosg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2oyedttbq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vcsiprhw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nbxnmgov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xuxuzaeu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bktnrtvb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjrzpg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vkcwyuiw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2knnkmewz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nuwpfnvr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jfohouyp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pmgypdah.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yvwlshdt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2fqlrkwhj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2itzsdfke.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rrqmozuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jfdycmvg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2erkfkxnq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2abpzxkql.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uejbvnys.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xbojejgc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jqrjnxvb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lpbaspns.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wtovoikm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tfasopkv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bwvzaeyo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lidjemje.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wfmkhncl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tzztzkqo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kxdlcjwf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jneyqzhc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bavhsyqh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ntryunvg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2spubrrde.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gqaxghmw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lzptguny.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ijybwzov.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jrnzgucn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2odulcnid.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vcgscpqk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nenmqkkq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vciimipg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mxzqddln.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twxmfrrn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ffnwndiy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwtzgbpt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gokzyzyw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wbgcucpk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2oriqaguk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tnajuhtn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ttazksmz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iiakuidc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pgifklxp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kyodunls.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xplwhxnq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yiritytz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lelzwcor.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uwbwmvym.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xvsyfyzt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pzpcqlni.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pgyfdyno.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kscwqjyh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hvfnsatt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tgywnxtj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lknlypoh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jbejpnku.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2psbvqssh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ruxrwsmy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qkddlijm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qsnhudly.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wrnchrjd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qccwnuug.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nzfxuyhn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rkwgoytc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2plpxdmha.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dicjvoqx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qnsksaoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zpacvyuy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ijxerqvl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nxuoxvlx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fiftkeot.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdevchmr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2gxhwrzym.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxhzeo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fkncbhal.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dmkaunqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ckymnipd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vmyqfyyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gwgiqfcv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xfmfafwn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vwpsgrin.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kinqzrqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scxcrqcl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxqnqngc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juzaxoiu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnibveqs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwvdckf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2idhnznny.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ouitbywl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xzhoyagl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fseiqboo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ggrecrnr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2oudmoaub.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qcucnsvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2secpnpin.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oncjkktq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2moptwicj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2aiwvdyry.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2qyzevhcx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohbxnqfy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2meodxtfb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2luoejioe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qxosoypt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2onbmqjfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdlqqktw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ciegisiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apngusnm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yadqheuu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qekeiyzv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gqfhrrnm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cqueevth.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2czbrlnwu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yitywgrk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2unrpafuk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cedrrbth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2czzpxaln.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2aqdkfgpi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2axlogqce.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qolkupya.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eibujzhu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nglcihoo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xyncllny.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2czsbzdjc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2asisoson.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pzacrdzw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iheswbla.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xxcfalfg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jbcgbzyl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oxgvpzak.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xzaseyqa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xsskrige.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ttpjlemg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qysrrwfu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qtspvxox.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxcjrm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fgkdyuri.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2svjpmhog.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xjepbbxx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2cplbttza.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2exranccb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rnwynfll.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unhfuusv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ffxjstmg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uwunbsns.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2esglhiqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2splbyzgl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bgiphirk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qleqtgfh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fzoneyrd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cwogrssh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nijczura.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bfduiony.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjnjksez.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rtptqljl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ieuiuill.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtapgocs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uhqhyrqm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jtzrynva.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlgvvrem.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqlbiiie.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tzskvpvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vujfsffl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rsxacrib.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2immzadng.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ujmaqjvj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tpvicrrb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2smhyikmh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2indsmlqb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddbwtmaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hkxugtta.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kjwoydir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2awrmavhw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tjdyxygl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbedtect.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tmrrqwln.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nudlfblq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kqhgjsrn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2opxubjex.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zqisxons.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qslxghxy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nreircfw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vkcjreni.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jmirhwqz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2uwymamby.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wgmggeeo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2usyvewev.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xuffgfrl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2duywyjlq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ptlgilkh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sjryflst.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ygxzeiuq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2micfctrk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tvhnferz.html


<!-- 参考信息 -->