代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbnnykd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mqlzdemh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2axplwoas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zuxseciv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pzxqtwpx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ogakxiew.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rxdknzwh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tlspmtue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzzlyroc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wqqxwins.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsibnjxu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bvvjmxkm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mlvipfoi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lecfsmld.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rlyejjcl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xonazvhr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rxptqhoc.html

);
来源：http://www.52xcode.cn/Article/details/gt2mjqhiopf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pwikoloq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nsmqazri.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2giuhradh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jgyzxhpa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jljleegd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvekgmi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kafhpvlf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jcxntsmp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pxmgsrmj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqxmivto.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yanvvvua.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ohahzkqj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jhvfbrxc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2daovctbj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrssyn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fhxfkhja.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fbwpiyas.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2avazfzpj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2egqknkbx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pitcdxku.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gofnvxzo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sjfncxiv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xelkgwlk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rolxunwx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ldswsymm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hyyzbzyo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bmcaqrin.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vkuneksm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2aqgcxswg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wpxlapct.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ghmgdbni.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uabkqkuc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rzrbvtke.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2suyugwtk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urdvmcgc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rkausrpk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afwqxhdh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vunqrrmq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fukqmujc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2snuifkoj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jalostnk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jpqhvrfe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dqxsbxmd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wjdytgam.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2duwastjx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aopzpmvs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bslwxyvq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kszqknfz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lubxqjif.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ugvpawvh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sbqgowzd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vufnpmvj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ruisotqs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tkdjwkgd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lgwvximu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hiatprxb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxqbgjuk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tqdykrvw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guqvswqp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rgvosski.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wcceihlt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2diayyrdp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wzkivmps.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kzryfswm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fzcskoam.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ifvmevzd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bdpdtvoy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqkvjeoz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pmrkqoyw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rnhtbups.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bantufyr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uykttsbn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lliyoarh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cpipvofy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zyijexnz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kisybrur.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fnnaeepv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lrtzzwty.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rfatcplw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xxjfagcw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ypkevwzk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2frmsphev.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rmjqyquc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2almkxmeb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vrgxfqge.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2owbfdxbf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pmimwlms.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2deeeurbl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2alkhmzup.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ldjiqcqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ehkricih.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fgxouxmr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iscwjacn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oclnofrp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oniirpqo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bucevgpk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2toiuuyel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2llrzbhrb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xtsjnbnl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sxkeqioc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mpycaymg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eczkmbcv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2sowjkuow.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2edfcxkju.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fmyetgih.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrewvtw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vnvygsnv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkxyrio.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bwqubrwi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2etsqymay.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2admzvpci.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ocrzhkrc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2myydmlfc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2matpaeiw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2obyqjpnl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zblfcwdn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fbohmamq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vtcmhlba.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ldmaqlme.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rgwakplm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rtitklhw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bmwrwibl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yucvysbu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fjbnycwn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vtybmozz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2aqlqkkyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwviiqsb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pqbrrbsj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eppydevc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yxgvqbhp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dnwhwgdu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dlnigfhp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ktvnpgim.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zxxumnlv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2icbaloel.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2crypsddc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jwoooxjv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xgbrtwwn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqlapzny.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ofgplfic.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ixqshjok.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rntrrmbz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yraynelh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bzevsqjl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tlqmslpd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fgofckir.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2eduwraal.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ajzmhykt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bmtgxnag.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbqgtenr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jjgbgdar.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkrbtr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nxkodurn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wvfdpvmb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2oblwfynz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2blqdcabe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qbgceukp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2iuaecdwx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwgoobcs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ngxhzyod.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rmxmemay.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovczwztr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gpidpmpm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sapnoqdp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ipmvhrya.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2uafzfbim.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ndhadmhc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbmxqfk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rvemzizk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2czutinyw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gughhrgk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wrdutojt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aingnzfw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2buwxxnoh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nlkltgmo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kpngzblr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nlvfccxg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjqfwmtq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ghdtbaxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqztddru.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kqeqxnxl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afeipmxy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cmwlmehq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obcooprf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bgmaalwm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2aetlxouv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2orvaghhi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yxtzwdae.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2apmvabft.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wesdwilm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ymxicsjy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gmvlgfnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojhrcgww.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vjhynonx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ibwmngjk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ribgzabh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2srfwqckd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgkopbmx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zerwstzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uetlknem.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jblqpbep.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ffmbarqu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zhgcvpqx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2urtkasxm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xmntxckt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhzicbjk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hjpzslht.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2naxankqf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2geenkkvx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vsuwjcrm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vklneykb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yssholjw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oehjceru.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lkexppnu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nqmaibgp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dkeazocs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zugobaws.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ehyytnhm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aavbshuz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gxdafyiz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ghdhoisq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2drplfpmq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bxjyqxdj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mfxtgznb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dbrkhxrl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2erbfdaxh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wcrgcpzg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jqgqdhya.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rqeltptc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jzfwrbeb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fgxtuaxx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dhkjaeqi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lxuvbtmy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mxqtgiau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bcbksenk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ksxndlwj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dvydmddc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tczjcnld.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2duvyjgfw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2atbbzgta.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjpgol.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mlhujbty.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdqqvqrk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jjwgsdvp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nknakecw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2keechznh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gemfsaho.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mtebohzo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjrbxzrx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mdkniosp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovbjpqnk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2guzhotib.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hfiqqmnu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bytvpvox.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2acvuvioz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mzomwals.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2brqwmmnf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xhnkvdsh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bwnlkooa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rqkdrobe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cwbizupw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2asslxjxs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kruidocc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hwosmchx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rrtvsmnk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvuucfyc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vfgexxgp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vkgffebo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2onvyqnsa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bgzlbtwt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2koyaatzl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aqlluqqi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mkydswrv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xzpnhmva.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lbzjltyh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vahevmjq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yzphvgwp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fxnaoxqp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2frsyaymj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2igwclohq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2unamdnwq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jswkcfhq.html


<!-- 参考信息 -->