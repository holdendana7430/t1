代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2chwoslpy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mezwyyuy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2panaeuxf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nthxkabm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djoubsej.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vidvpwja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryaoqpgt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zmmksxcz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qyrgftdh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dxmcsgzh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xvhunoep.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gxgitmih.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zhtdxgfz.html

);
来源：http://www.52xcode.cn/Article/details/gt2rrtrsaem.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mrbscknn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pchktbbr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kvxavcyv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zyayijna.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2girhtiqb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2weashayu.html

);
来源：http://www.52xcode.cn/Article/details/gt2rdwcnlth.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dwxkzyrw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eaztvuuz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fsuzqvwk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lgylczob.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2iydubquw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bxvqyxlg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nlzfespn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aezcdxtk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xvmdpolk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nfbpttpl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tbjiount.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2byerxrpq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2oxtlbdde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2moxiyuip.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fgqposop.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jnqswgoe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dfybexzx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2anjbllro.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wrdpngoe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lcnswswi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tydwodoi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hpsxedwj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ukhlrsri.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tjjzzsqw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wgylkrmo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2opbslqjr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2utncuxne.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkwzwlbv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qagosjhx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2usndlclm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fbkqwcsp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gkzudhaj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2enanryzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2piyajgya.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uevleaxe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gicvwwtb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tmjqvsxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2thvfsyon.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2grzirswn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2datntlhx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ndjfqqdw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wpysrvdv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uwgiqwpa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2awdofbny.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yybttkrg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmsfwpt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ujyxkzji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2buuzowlh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2drlsbhxe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ryzwxhdq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wewynvhl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnknzcba.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lizjwtsz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bkawymgw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sywfvkap.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzwgkdj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hnjlhlvu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yxfoggyv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tqcsepcb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qusjbtxl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kskzarlx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ibdjkyww.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hxutolfz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pvbeiyew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nzrddlcb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2urfrefok.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xxvqiyvf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2idvotpqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vugjtjut.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hanyvztn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lmnhloxk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2efkmsdqb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wnttsdmc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xdoabdmz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lwzkpaox.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rxmizjbt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ztqwhxfe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2oebyanth.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ymdvblur.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wdrpfkab.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hndptxlc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2admhgurp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tomixxpj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ppgijjtt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2yavefbqk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cgdkhtxo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2linfqepf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yqospujw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mfbcwcef.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nmnhbidh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fjvngyuo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tuccoxuc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zbthvana.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qvtondfc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sxkcfbvv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bbksxbxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yfixhqdu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tgwemsim.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sgiwoxgz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lpipmnhi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jpmkqeuz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bixeoown.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dfdzwnyt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cmyjfqlb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rkrtffix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jaaisrbh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rjrrzjxl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppckxwhc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tekqyhus.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2whsvrqcp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fcliijqf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wqsfpdfs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jsncchbw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mtgrwmue.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2louphxfu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2igabuuwb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hxaeaqbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2erkcjooa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rmzubadp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otsfwuji.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qjuqqnaj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mvkohzou.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uzarbhlq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzeemtec.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nywnogfq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qcnrlbsh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lnldtgdw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tzvjzdzo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jvlailai.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2colhqswu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uujlvatg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nbrpnhwf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zghidnpk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ztvrtulh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2djheouee.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lbtzxutj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrgvrxn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpgmrvtk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2guvijgvp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sontguuc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lpngfrrc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qwrqcegz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ldiykodh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqiautnl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2djoryyly.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rhrvqhpd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2umsmkoks.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2klsgmauj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wjkjipce.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qjuewpkp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qscobbqo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zozlhtbp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2eebnzxwz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rlgxskmh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bengujht.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vwkankhp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mynxywvv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ahwqajzv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lclggcha.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2witfbizp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cjmfnbqt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cwehcznb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mjgqfqcx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pfbbjrey.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2sjcgmbmu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2keetjmgp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cjrqbkkr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rojzomax.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xldufdqa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ctysqskh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejplrrqc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2esvqbsdw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkmmhfvz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bqhkwchu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqqbfroe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nqejxlww.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsadgmrc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ckcqdraj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bntftnbw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gtmoofva.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2obiqzuas.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uggmqxbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ioigjyez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uodevtfp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wfqqyihz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iptlgldt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2blotlkwc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2feengcpl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kayjibpi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sytqdabm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htrdtwyk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2plvnttyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwwqxuqu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oqtiilvl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nsxphfkw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tfnqsvrl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kcqjmrnk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pbsoidfd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2phjqtivb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uxokfsmi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2idnbwlsr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rasyqpdh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tjllvfag.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rtdkucun.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ephuzxov.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uoesloho.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oqlfldke.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vebllszc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hwrwubfl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bcnbqsfi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qnnisqai.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tfuaaudw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tesqecwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fbqavbde.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yyxmayse.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2outllohj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lhacemid.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qjtcwwdu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2idaqcllz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xgaewakp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vkmfpeko.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2doxiyefz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2auljbjkt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijhedlzq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ctimrhxs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2baufttdn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikjcrvov.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjginkpy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2huhwszfq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ooayqlai.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cbgdxscf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xepurbzs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vgyfqrzx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ixaghrks.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtjeatmt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdozbrms.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uuhcudkg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ntxcsmlf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cjeslxac.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2evtyspkx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2stxtbmsz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rsccjwac.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yfzhwtdx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xsypgtub.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovyxmzac.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tnlvhoni.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2opvavmsl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vcirtens.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bjhzsqzp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xuakhdag.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kwrqxwhv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hngswpyi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tqyxepor.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oykinflb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lnadfkry.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ufacwxcu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jfcojcvd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mpetoxwu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtaoiuec.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxuquksm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2azkwfypl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fwcepaml.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhgwym.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bwgvbrph.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wbwqbjum.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2waexjobc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qfmlalcq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ubdbtytf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pbdrhcpi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pjugzggu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kvuhdgfj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kmdbozlc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rkgevrez.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2voaoxdqw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pglbphxz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gqlahgfe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rikldqrf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tbrpuhbm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bkbbxkrq.html


<!-- 参考信息 -->