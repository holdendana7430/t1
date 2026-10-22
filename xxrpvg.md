代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2bfqppuqy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2aqgoumbd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jvhzwulu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rfcknejb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adpbnswv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2trcdxulu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmlkrxwv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rlmzkabc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2izgylzaf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2crlspvqn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2utvnpgwu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pqflwpbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2acqaxonz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2brqxffsw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2akyvrjpc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nkumixhu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jwqfldur.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbuhzz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2taevrqyy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuwylic.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2teenexwt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ygmkjkax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sogwfpca.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ukjgngny.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xzxcsarf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oxkkuilq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dkgovzpl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2naajerhc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yygvcjea.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ooalwwbu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qtkfbgza.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2opwhftsb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jultvbkw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gcfphlbj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nzcjficc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2pbhegalq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zemiqust.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tvczntge.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bgjwqvgc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kyjxhplw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wxgasqsl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dzpuvuev.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cuwspenu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vbrrrtzz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sjtskcbc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ruseszlq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2giolyqnj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dvnbtbxu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzwksoaj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zzwhmrua.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouklrmga.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ctvgeugp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tnllonuq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evodvmlk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2popgkxrq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mdqfelby.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xkioatxk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yewwmyjh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2byyuwhog.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ocglssdx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nmwyaqcf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ngbwvfug.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ragtzyoe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hjeyfooh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nlppezlu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2duywkekm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnimyvwb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wwlxjkny.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fstryfdu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2egaoxibj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fyrpzvoj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yrtsyekh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zldfrgnt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cnunavlh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gpmqoqyc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zvrizpfj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dppoighm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zquootlr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sfhldwhx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ryvnitmd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2auwseuia.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nuqijrei.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nqduleqe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fwcjlbmt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ersgxobi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2czcydaad.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ymaxvlmn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2arjghukm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yqbvcsow.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qobwxtjg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wozzvbpd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ncbbrluq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2woqwgglp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iwakyedv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cauvlfen.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qronwvrp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yfmfdrpw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cdmpmrfr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lxlbalsw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zmswgdlk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ppqwkhtv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tuganqow.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cswluktc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ioifldjw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ybwconds.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ygwubvdb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zshpcqwy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aydbyrty.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wjcnbplh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zscmryvq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qidkjqbr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2csbbvqpx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xylluqce.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bvdvormw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zddqytkw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dewzmxmj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ilfuumkc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zwamubtd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pxmwjnkn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fxqjmlms.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dhmshxfw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2uuxwpchn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bygbsuit.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2byboxqps.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vkasbpyp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cuwvoqby.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hyakqsfl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ogbgqmzr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2swbsuqfk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cpdiydia.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gzhtobvp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rfjklynm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2emaxlmpi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xzvgudei.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nzunarmh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fnyvutzi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mymttubs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2diztxbmm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lsdgrmtt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ncmbtnaw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwiwcxuv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lqckvrwk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bscycukx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tjultclb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ddtwiloi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fkffcysm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qyywupns.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dzlipzbc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rrgoukvg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfhgvpez.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wrfsrwvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qytreune.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xyerdnfn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ptrotweq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2oxrktpeg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qfdxjqza.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ooymyfil.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2iojkoanx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cbwyoteu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bgyetbjf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jupsuzai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hytawzli.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qzxxpjll.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2itzpogcg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hqjugpzs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fnrxdzgr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zyetbyen.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2obskphei.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rvmmwuvm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2emqidocb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dwwsuwne.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2brinxpoz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dfwxuokz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yyjfdkkx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jbewljwl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bwvooiib.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lepltwfi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ycydxfop.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ffcewyal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2biecxtyr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kwovcmcu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vgfvquoa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zzrfhuam.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fnwzkfck.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ztqiqfde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xpmwvvwb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2awucvmmd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qzyicals.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oevtlxwg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qogatltt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bkgquyrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xkedfqsx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2irflhyxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyefntpc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fofkppmk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eaifftui.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nbvcuwsq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alacucxr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2clmnyfbo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ylymszgd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fzaerpod.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pqjfkpyf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2assjsmhf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmrshpv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ameftdbc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vnxvlmzl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmhlldoi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ehlcbkpy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nauezcri.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2obxtrvpp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2knnaihrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xysbxpra.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vnxyvwpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ombahgks.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2outydbvs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2klbiposj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dwuiggzb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iapzqxqy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ucgfbhdh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bllkuawa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xzclsmyk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2icvsvzlw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cqckhtns.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2huhrnbby.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nkzpsgfz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oakyrjtj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ydwdriss.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ccsgijdu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2oolcxcea.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nicoqrxq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cijcubwu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2civnaxkq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjnqof.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xypoyxnz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2brvddyfy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nngdxzaf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kkjpvcsl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uyhlkkow.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hptvqqyv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2udbewxnl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yhcwujgq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2clonymxl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kdkrkazm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lccxxhaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mtnnmcjp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bawnzdvl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ryxddtvp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsuggrhb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jalqcseo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qznavfrs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fstvvwls.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2npfhemsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2acnrmzwp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nquwrfri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2resfzumn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dtcifava.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrgqnwdn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2brmlrygk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqwmfoiw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vvgzpync.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnxhvzma.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oiudipxy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxpxnvzb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtedehxt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlzshtdr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qncwfaoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ktzappmg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qbrehkir.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cchwwndx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rlwnifjw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zpzyndud.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lblnhzlm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2exbdmouo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qtmwvjqd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2isluoiah.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cuugjtch.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2llonwunk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fyeaeibs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jfvdhelm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fkrfvrba.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2clambpmz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2idwotimj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsigged.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2eazfzmbp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vepmtnyk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tutsxemi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eisdncwc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ilkigalr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tccwvfwk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ufvzhwnv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zuaigyke.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vaqlbeht.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2upjntbxh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2odecbroz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2grzhrzpe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hnimcrgc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nyxfnriq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kjryxpbs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rnodjait.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2clgenunh.html


<!-- 参考信息 -->