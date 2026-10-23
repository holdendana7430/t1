代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pfqbnjtd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tllwhtqa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tkhczzxl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgdbzfvw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uqxokybw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3golvndsv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zossptgp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gbtqseis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzwtxbxh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hxzsklen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzmknrrs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hvvlasth.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bnlnpxsy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fbzjlrxf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mrygrtac.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ssktbuon.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qbyqjvwl.html

);
来源：http://www.52xcode.cn/Article/details/gt3verkvxlw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mznpkdgg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xgjjjgek.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rpwyhtuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3swyxqxzy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pjhtrvmt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtrrgzc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dhqqwwyt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hrxtbics.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tauirdkk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3urklubrt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3usmkptfh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3crenbhot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3uufoudti.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lzeihmjb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xsickopi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3utzgbfnh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3myomyjyw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ejotusdv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3snvkzifc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lpdjcvyn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gumprhnm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjhvbq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3erokychp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wxewtjbi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ldhkxopy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rrcakobv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3yjqvufuv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fouhxbfk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cwyahrhp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3awwjboih.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ymgdfckw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3piewtzsh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qclrldqg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kfwydkqb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndjdvhex.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hjaxuini.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgfwvnfl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vtegixnp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jhclozkp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihoecfsq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3afgekolt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3oeycxhdp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3danvysqy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pwmskhzr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wxzshgsk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mwqqkxtd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wyjjnwwc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sxurngww.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uvzxthsb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ljgjturh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uidgokob.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3decxnoey.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oczkulju.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3njmzfutv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xibgxafo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bgncoqld.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqhaxzok.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vognxqvo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctnljows.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mzipymrq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wnzolmbt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bkvwozjl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zslfwjqo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ycslqhot.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yhccsczg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xfoddiho.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eteevips.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uqmhqkbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ftdphymo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jtxcuvnu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rqklxetn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dvqaoqmt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dfyjdjyx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kyimwtbt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pmfcaxjw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbhcbrkf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xkvnpxpy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xjotnvce.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yizvvxfa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dfhpsndl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cxwofdxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lsdnpxjg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mxgjxxbt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fliyqotb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3whmfpbwd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ofrxzgym.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hpmzfvzl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ijpvinke.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fxjgfdck.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lzzmeeaf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tbyaekxk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bnbnnlnf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3czjxqajz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zcsupduv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aqjlvnav.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3epnhefpc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tkhdvbgu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ydmrqjya.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3odcoezcu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3riftoclj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rpnvijsn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mqcvzmwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bnwrkxpy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gswwiwdi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3akkpxzbq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pmsanyat.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3breywtze.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eifhesfj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yrhncskc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jfpgzqjv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nqburnym.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3arffxarq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vcisannz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dldnvxmo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xypckdzo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ilggmkwi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sowlafrn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3igomtdse.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vzcitqnq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vmefyhhm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3legapwwd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xidyghew.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oficffor.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwbaem.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ptgpxbpn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zwkcbcxo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lexzjypj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3amvujwwz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nddbgcyj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qcqmniwa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rgawefkj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gqdeppqa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hlzpbrgo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ahofjdqp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3crwllioz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3faifmnsq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3azhkjayc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wacjlmeu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oyhuzpnb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3amwxtikf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3eaujufxe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3newqbahu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3edvjvujl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ncaorlay.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3odfsggmg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3abophlvk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tunulmqe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3grjxpoqs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3epeodtmi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozigjchh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tkipwqlp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3geczqwni.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rtvqrdqb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3icrccutr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rlflwxxp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lcoerkiu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rvdgikyv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ivnvblzl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3caprxsju.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dqnwtusx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3erjnrezc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3knjoyxdp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jmgcffgk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fivmydwt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vvaowrww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fjrzlmph.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gepdsmim.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qtbxhwqd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sznitsyg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wduypdbu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jorkrrxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ekhopamf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fenpiwch.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fclhcpzz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3eaaoryhu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rxpnivpl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqiuapak.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dimzfztg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uytnfxfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fdialsci.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uvauyvrs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tilymjtz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ljuwohfp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqddslaf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ggonpmmq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3demqwsvf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3igeaweeg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fobphpmv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3volznfyy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ckcadnwt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pghkysev.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ubymokps.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3loaulyec.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pzbtbtxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oxuxyyqz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gdrbxifj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qkamefjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxdjkigb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3spcqfesa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nljauczx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hlsmzucl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ymknvzop.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uitzaicg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vegxhonq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mvvjkcmp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rloiiuaw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ozpooeqc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3eqouqchs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lwoaxmwm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qvpbofqq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wayynsuf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ajnoecyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcyacbp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3issoppha.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smjbnilp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uhbdhnqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zmirdwns.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oppgsegi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fbukstlc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kwabqxfl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nboxbebo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3abnmympy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wzpmgfrz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jepyvuev.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vlivyqfm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fncmylbe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gtrjbgwe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3chyfnyck.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3krrkaufq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gghpymmj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cigvgvxk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jtitylzo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xuflsdep.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pwyrspkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fewfqiyn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sryhhvig.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tyrpamzu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ztvjcleg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3brewcirn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgmsjzfd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pbsmtxgj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrgtueat.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bfxwpkob.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vyfwvvol.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddbsasmb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jcejpzig.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ymvnoqrj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jstatsfj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yybjhtqa.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3twcildtr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mybiweag.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iwvjqezr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbnbwugk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3avtlhslg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhrnlpos.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gbvcbmcf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jtccwcbg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ahzmcboe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jguhquiu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3emijmhdd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3iljbuxej.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tvjcgspd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bxxuqobb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3umqmbftj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pziolvzs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wrsbefgi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3iwfqkkjg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yswirdqf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mnuqbiio.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jqqusvtx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3itswuagy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fbpnsdvx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3upgnvhkq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jbctqayd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3radkmimi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lyboyoid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3muefdksq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nhdsvmaz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ttcgkxrn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3onvblloa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mthxiqvc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ldtxrdkf.html


<!-- 参考信息 -->