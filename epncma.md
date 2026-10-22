代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rvizcrwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gtkcoeic.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gyvnjeji.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ypujdtrv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hsdanual.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2uwpukuwq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2clvphkmp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wsdzwvpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkbwflfi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mqzbeazv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llwngyvt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fgujwpie.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jqmuhzbg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hmvhpijy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ossmvlhr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xfxaykpz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zwlnfnwr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jzupuvge.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tldiddec.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2liadawer.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2syqfndxb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zyfttcqh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rieszljp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lxidrmho.html

);
来源：http://www.52xcode.cn/Article/details/gt2mggcdmej.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ybekdybo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ocwslahs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2khrqnnsp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jqfghwpf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nrmwqwcg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ivdnrama.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xptempur.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kvdgekij.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2exsdwkft.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nluefcnh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cavbwhjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wflnmdns.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zyyawjmv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2djibkpzf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vfqysvll.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2youmesmq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2juzlnnzw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bidcifii.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2oxptaylz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qoivuecg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wnrnpcfh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2khrmjivf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jxbflles.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ufzquwkl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jpnfmgep.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2grngodsj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zspwyoag.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtcnpfvm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sbpzoqte.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozoteutf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uppbsayo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsabpkeh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rsmatvsq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hksbukan.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yfllyitb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2oqljqnmk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zrznnaae.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zykxudiq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qdbngzit.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nvhsiezn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2keibqxlx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mcszfwfa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hnzxnjtm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yfnqhsdw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2alngfaxs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eymwprlc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qyuwjlwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jzcegfjp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wdodcvfr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anqgnafe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2khjkgjoy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtefzsjn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dphytxeh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wjlcxyjn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dstpbtap.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjvqqlwc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yinhvufc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wcjzcojv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gucovcye.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hzrvhahx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lphkmdni.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2deuugrsg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2elnrydbl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bczzxawk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rdaxrsny.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2pxcnlhkv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dchcslwo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mpctuyyy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nxozvyen.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iihvbymn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qnuevwpp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nnohktba.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zlnpugxj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qhqkwwjr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xaecimcp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2enohnawg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lrhngkaj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ufxhibfl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xntslwjd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nsfbktnz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wcwgkadx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fcfztzlh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yyxhdaqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2roodcfjk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jrtqmsqq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2opxirzhd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2olcjywzn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lfnmbugl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2emukntdn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jwtyolpx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hbwrapzv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dbwxvtuk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nuhvbxrt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqbwtr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2whtneked.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hwkabmda.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2loisqicg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jxuyskak.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fezlgibd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ibgshhmk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zfpqxgxp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lacqsaev.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wagouywj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jqpeqlit.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ibilhivj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dkgkgawi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2unpoeqnn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gxevdztg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dgnxayly.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fpdpxkzx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2lowvuucx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dlchtdiq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nycadsac.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ueltsslu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vqqrjpcr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ngvieurh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2apoagqyf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ksgbonyc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vyzheggf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nnimhdzv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rjtxirfv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wvthwgqn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ajrsikdt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kefwewdt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rmjisqzc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jtyilhkp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zvlasqsr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iirnqyig.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vzlrntgg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kkemlaly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2raffaplj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sunpexwl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gauykmyc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zbjhbqdj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wllmikkz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ayouzqtz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jgmcvngc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wzpzpzcg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xyecagiv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bzjpkbwj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2etumvfux.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yjtsoycs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2buxxmqum.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cfgfmgfo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zypwfbxp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yjevtckc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2eonxbqcn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgckyu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bxjqgoch.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sicjlwxi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ayusbgpg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvvxnunw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gyjfoczu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rrcmkjni.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cygbjjte.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2esveszll.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gsttywcf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oaagfsbr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2sstnvnhh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nyhmwhcq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2seifkvek.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jlucvbxm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2newhxvjq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cmenkbke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vihdnqya.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qvsrjcpd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xqwvwido.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ucgaqdak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jggoxxmz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mdrygfdh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzymilnr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ciftjaak.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcwhjk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rquljaas.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xcuqwboz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wunwgmcs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjsdmwlt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nucdggkc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2awulryuw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rbtcjtey.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xcfnscmr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2henerwkn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2unlexxtq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2galmmmal.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zibpbcpy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ockimuei.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2catqtmfp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kzrzeeon.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2neyvoeth.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpuzvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wupqojye.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bygoqizi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npxdtoop.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kwjphuxf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zeniqepv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2muqkdqrk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hnafvits.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gvhpnipa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bwjbrprk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2csouuyex.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qmzkivmn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uhelrgwl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tumkjxat.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqmancde.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jteluwnz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vvdowedm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2florrgpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2klsbneju.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2koctnkvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lsaixnwf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynppqzpk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aycikfiw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qdtxhjay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pzghfpci.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2aixmjqhq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ahqtybtm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yrytptea.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2chteobkb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2safojgnl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2efhmmlya.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqiurcds.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2djkhhcnu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdsujjhv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zwwgissv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bvyjiwiv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2glcwyybv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2odggpbkl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vlmvaggw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vwcahjly.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ckyiheqi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jxvxedpk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wswbhrrq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hiefavoq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ivkxsilp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rvttgsnj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mjbrqfak.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hvccngeh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmyyback.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjspnfuj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kytqlvwg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fzscncns.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jhrtyrkb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljrzuvqk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2attvxkdk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wzbdhclx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2inxqqvpu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gawhdrom.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hotjsllk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2srdhvwjg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ueywdcoq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uhvaubxx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mtuukwhw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vkpnuufw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ghtfuaia.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ovshviqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2uqdxoopr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ysfeupkh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2liudhskk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dsrlceln.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hdovacvb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nujqzldi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynouyhkh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hscdymaa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dgjvfvkn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2phwugeuv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gixxvjit.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cedxzcqf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2epsvwufn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tdqcmyqo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bkmgwyhj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zjydjvcq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqjcbsx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lnvqbomq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2larvdrnb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dwnafhda.html


<!-- 参考信息 -->