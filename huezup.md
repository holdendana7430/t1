代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oslafqab.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lovpqozw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykobkxer.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kdrqhgad.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vtpqqyay.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oxcboaga.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2prichwjp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dpurowoc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dapztevn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gcuetnsm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ywajajvq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ewfdvmfw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ajfuhtzw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2venmslqc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yygygnub.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rcnfwtys.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nxzfakpv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qetujtbd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gvimzesv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2apqkpztq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wrqpqwdy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2sjrbzcto.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cvjflmvi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cjtjqsbw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wbzhlotn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2aokvnnta.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mtbsqhas.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fcwxplux.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eqrlcwue.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2uyqyacgy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dodslqpc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pfihsrsx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qwxnbtaj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fiumizxy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mkkuqyvy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2icqcrqft.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hytmdzmf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ghpdzqfe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nstnjrma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2suzqzdhz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jkjegskx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ghvllmks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dkcblidr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uoetaawn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njvuzvnh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wgaczcyz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvqijyoy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2drtiujaz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zaxvvmrc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kwzftjba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bxhfeanr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qikivhij.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ktsmrbrn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2slwlckzy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpsmzokr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uwibeyaj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dfgzavkg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rvnhzayk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ectibiry.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uwxggzha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rygrboey.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yvkeziqz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgizuwcy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xgqslwww.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ibhjrfxg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sriuvrds.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtfticco.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sfewlbbk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2evxziviq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qcnygsoz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cbdzaols.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2whblndlt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrsmrmj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iuyasplw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dmnsaoeh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yiuafbea.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xjgsonfg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wjrbwryk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yobsxdmm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mrblwhwr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lvaatgty.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2aghwzlhj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2yvdepfsc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sqmsyajb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2freihtwr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xvgxpwbe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lpjzadxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2owrhsqkz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2frkezyxl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwijgf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uwhhhmse.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2slkikdyy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mneilkih.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kquypsau.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lcllrvvf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sqinvbxl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qkaxxoko.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xjhshtgq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2toilhoot.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rtmzhzzj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2feikxchx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lmaerbvq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hyxrfsxm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aiqnsope.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xdwarkqe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ydcpjzvv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ocawedig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nvfobmiu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rfpzbipr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ghvvkamy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wtibuwmg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fozyhhjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ylhgshhs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sgojuojc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wpqgcpzc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sznbmazh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xeedzpae.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2axetdoln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cekadpdz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jrqgckcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xpwfgsqg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2euzgbcdn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jahjpaiu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jpktfsbx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nszfbjvg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uiebvunt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bdhausuq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ctzoziuf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ryoorsqe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gwbylibu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tucgqyno.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mbrptkvn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ngpnyasa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xbohwuvw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qbgkbqby.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mcgfazws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vblodufa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nyuroors.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2harpzmwl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hmxbfrry.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2crxvkpds.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xxvfyodq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lzaesbph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdpsmgis.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xnzxvuzl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ubrfqhdq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rpttjkvs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ozwwpnzj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qnbzercy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nkwdttul.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yugoxlfg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2pyledwoh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2peutwupk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2yirwlhpe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gphxankc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wrimwrxt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ottqordn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wmmquscx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xdkqybnj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2himywzwu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2csneiiya.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fcwpifbs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2umqisflf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2afobnqyo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2axjvongn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fdczhjzu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jptxeihj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovxbwrke.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2darftgmt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2usszwbmb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ushsuhgo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ifuyuzet.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qrrmcuky.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sowvcufa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wkzzsoqy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nzxnrrud.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ebvnpzqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ehuhocdb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ngbfufmu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xdfuxliq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sdhckocw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ygcrwfen.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gltiiphc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zsizexjp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qqqntgqi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auomlnuh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcyogzvb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjbonrnm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mbzpnrbp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjvforru.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mndqzfpn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsiqiwfm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2epzomhha.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vliwuuyr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wqogngcu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lrxkmcoq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zkmzsoer.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2uvbptlzh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bkwcmuus.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tzybdcnx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lyedualu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ffvjwynq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhkbzrqv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xokwnyjv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qepjwshb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ewpkielg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hqodhmyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnlpszop.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ytqxdcvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uecrfsdr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pjfogfix.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vcmoagnz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2smtevzmd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ucpbzpmc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ozrlauef.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ifuisdrm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2kdjxejeb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kzcjijqm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nlicxyom.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2panyvdrg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyiwohfb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2chxqbmpd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2acatnpcy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtwsynos.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2skjhuaql.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xotzfjll.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fzfgunuf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aoaeocwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ffpmdtly.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xbwonfgq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xzixtpsw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nqcjipup.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pyvfawhw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ekshjgax.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2laqjlvkg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fkgedqvf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ltzcvfrx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lviqcngo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bvellmnd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tvsekplh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gvvwjbdm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bxprqyhd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kvylbfrz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tkfgopfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xogkfchs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2trberjhj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvxddtlc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fexdcnmb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2piukyfov.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yckncaqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2egajallb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iubjzvts.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2caevudmx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gqpspbsj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jndvyacy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mnkehxlb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nypprrkq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2anxhwhtz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mhwagrny.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2irgsyuuo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2irgkkymk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jzbugcvp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2syfqrlok.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kufhuqax.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ffevkzjz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ppabxjse.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wycyqknc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mxaxdome.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xcpkdwtk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ojuglesp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rbvufmnl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjhevgmp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mnsytzll.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2biemmbds.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gbxdzuvl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfvgqtmv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cccejdwa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vqdhakwi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nrueknic.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2benobdbz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qjqjlfyk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2eftfncrs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oyfpiiol.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mptedlib.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qfhdnxds.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cyltequt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2leqsxbdw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2frckvmrl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtiagmxn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ceouszpv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2epnovend.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2frnikywv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bmjhmqtg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zokhzzwf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ztylwmav.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rcgaimkf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jwthclmr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rltqrvcy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wcdlcdid.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jkvsvmwv.html


<!-- 参考信息 -->