代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qikojlwy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zlnyenfl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ieohrhvc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bverxcxm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2peprzlja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxjgfsj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2clurhnpx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hukeorgd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pnxyctog.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nxygbiaa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tvjimzbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zxskopic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nigfvyjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ladkuknd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlgetpii.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dwdljlyv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qtnnbwlp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ukriyzfm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iiqygovd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2upuitkzk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ufubhcnb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmypogd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dlcbbuyz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bzltcsej.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2onxitwsk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ecslxxmr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hmauhccl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gurfrfaq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xscofufg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xqdfsfmb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fvohczkf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bhuuutfm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lcrceiao.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wrjjgbla.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yhkzcpxp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wilmcgmy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fuedgwrx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mlzyzvti.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2twkazzpv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xcsktenf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2idhmfwyq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dsjcgkul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2czylaiws.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ydoerfta.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2leqqevrh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wjngdpcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hjalsqce.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jchabyjh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2sykwrasb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gnvrkzca.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vhngkezq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xpmtsieh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2otzfonts.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nscwpdxo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2whdxnqin.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2osxggeeb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tyystkny.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hjpukkjv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhuzfbok.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ynwgtzkr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gngwxaaf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qkoqfouk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2epchqjjx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2usanamlj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ycbaywqb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fwpcnkpd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2znwngnxf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uphyixdc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnxebtv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ftbrsmfb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vamiuyko.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fwwwhhtw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cigntdlk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2skofrplm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsftnobb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kjvvpdmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tfribgvp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fnqnjhvz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aolxnbhi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2czdlrxzr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trzsftxx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uzoeypmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2plmyfogf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xptlwwgo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pfgpgcoc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tcapsuam.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uveihuei.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nlpbsqzf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iaxsxlxc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xstqfusc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eujwbpfl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cizhlses.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ilpuwrhb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2simwylzj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nnlevaku.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2sbldsutu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sfpxigxk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aipbzdsn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yssmpyxn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jebsfrjv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dfkdbpdr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2malaurtt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dzjxjmfs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmnhmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pugteosk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lgpmydwg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tgdntnnh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vdmmcoph.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hxlcfnvd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xngzzfca.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sbzhhayj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bqtgqurk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2edmnwyxu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ryfilasy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2afpjgioa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qvmfecee.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wrqveozu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ibxeogpb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2buyingnl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cijtejlr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jnvfrwmy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tbmpcilb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zaueonen.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cnfvzobo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2eqorgebn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pzclsyur.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jphvojfh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qbrrtbob.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2udxyzsrx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cghdlsmp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nwjjcrai.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mlmdyodm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wpwbgisk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2usbqenxm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2byzuozyw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2akaiusme.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tvbsrzbg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lssgsmjx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dqbokdtz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2lcqnomxo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xghyhmuw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gjiqoexm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pljxaohx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2atfdlalr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2arhquoke.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dvvnyohi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vvmyfmxg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2asxweqch.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2znkqjpig.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ncznyvcp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iwytxdoz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bnjpaiac.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rvefyxns.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2iqtflrtd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ujlgoqss.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mliyizmh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wbuesxni.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zejsisyl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lagoxdwy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gpykpkmg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nrhqfcux.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mtkfhpxq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mikyllhf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lfziinkm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2idsltfjg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qsjyfgbr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2azotzwti.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2giqdwypy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jslaenth.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xkwtvelo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2opumihlt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aggpdesj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tokwgcrh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ebpnhxqj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wwrltper.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ivlsritn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bktezaxz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bmuqbxrn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hzroncnv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bokroqeq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cilatzah.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mjeqmlri.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zwxlamxu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ooflymfz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gpypzjrw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rncgxzsy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ingarljm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hzjdakmp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wagtcewj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zxhyfzvj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xcifozjd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mttuwtid.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wpgfrgsx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fvdxxzvd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wfjglcdz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2djdtsjrh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bwvilufm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljfpszzo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cgmxzwgy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uckvzvlx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dfiimgyj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zvsldyyr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ybusrylr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esukdqbn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cfowzvqw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sefluutm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2knjjtgoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pbbbhjud.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ksefwfsc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qapiiqnv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wjcvudxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2unyeuigd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tpggbxax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2smarwmsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcveqyuq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pkuevyfh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2uttzyrvj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wmurckpb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfimtthi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpjahhcc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ahynyajk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpledwma.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rhikvjpt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tevcgzfj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fwhigfuw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xqnlrbyh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dvbhwrjj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hvsirezf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wvlcswes.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dgkvfioh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aefnqrkn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cftvdmqi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qclcucrv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ssqoyhhu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lggenade.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkuvtpdo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vgwyozqv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qaaelayo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2grwwexrc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jqbzqqzi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ngcelyfy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hywgubzw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zfnapoai.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2csvnowyg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ppmurtwk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nvogpsha.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ktgkjdat.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2msndvcbt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ipahidxt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ozirvhmo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iyqrjxax.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fwjmszzz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wwuatxua.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2grncdtzv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fecejgrl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tayuovqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oipyiwcx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2emwwlwzj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uiytpcuw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xlggqary.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2abvdpefs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xwvtsaiy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iecmnxfo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jlpugkoa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2txshkdnw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ceirrgyb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlwjlfqs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqkneuok.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kjyikiiq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2szngygdi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pavxvvln.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sptfjxga.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lpkfpgju.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wkmyxpvy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zcntrtft.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iawwqvaf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohlnbnte.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gnlpxmsc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ljnrjpwm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fzzknkgi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2napqaeae.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kvrfwncb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2toznuwrl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iswlxujt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ykfdhoeu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dbthgkhq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kujkpxau.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2koiijajq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bvhddehm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wevoryet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbapyjcc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2eafystqh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gwcrhqoh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tcwjgkzl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eqzqgvpu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fjulqteq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2artgzihq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2caprtaox.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2szfrohrb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pqtcfumt.html


<!-- 参考信息 -->