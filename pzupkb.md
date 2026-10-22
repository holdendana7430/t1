代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbbccov.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hnvhccng.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkczuvk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ffqxmnfo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wggcsisk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zjdlxbtr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xzldxqmk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsgdfuyr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zviyaolf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbjcftpe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2resgqtdq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2axqmkoor.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dnewhqqh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhbktx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fbfmlqvl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nwqnzywn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vydjbeos.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qarjyzcp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmvtzwgj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqhqonl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xbwsoftz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gxbtmleu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kajohuvp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2npfarzmj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmxlhcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2sorirqfe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2yiydfkib.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2quosybnf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jjxsvnad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2unwzdhuj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpqnzkm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dzorbovt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdomwrul.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ylwfxsbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2incycanv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vuwvfpkm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jbkfnpya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uyycmvxz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sesaldme.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rcjvrejk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nxektqjg.html

);
来源：http://www.52xcode.cn/Article/details/gt2rzbtoapk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aflgavaa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2efoqodch.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fyvevhgg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yibqpdwq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zcxffdxp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uktgaipq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbgrizr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ncrlbmhp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gnlcpuvl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nodylqcg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mbjcsxbw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gsnxdytp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2stghfgdr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2onkdflol.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lhaugxgr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yklcatou.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fdnevdwu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2riicuacb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kramdaks.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kbvyhymf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oazotfnc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uugduzfx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2amfwtrju.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2spcddaib.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2svqvcshd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vojmgshe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dxowfgff.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aiiawdki.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2imnhtfvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dlaffeby.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nsmlolmn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sibadbcf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2azbrslmw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cehobaep.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vasesgzp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dgunejbj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkimtrmj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xuoxdzqw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2itmgwaaa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lhdcztsb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ndacotjx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqvkgvww.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yxytosix.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vmbuhvof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pmmublkm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xjfosteu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2foqtbbbg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wabcgtye.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fmtngsrd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ltgscrjd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wdnmmmzs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hwwuqnda.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yizwhhkz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hmmyrjck.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pefflwrq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2arxpcayz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fuuonkyj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mtmpuxwd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggcfskkh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pcnjxzhc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ezbpblvb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2odskstlz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wyauxlsz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yvpwumbm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2velffepn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yurlxygl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lpurcfgq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjyvgvdc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2youibbov.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ctpajlto.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nzucalcs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dmplsvtl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kgyhikah.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wgedojtw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ytrasqdt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ztfotask.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vqjlstwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fvytyuou.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2azkxyagp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jyfaxorr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wutjgdnq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bnvqiwle.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hzjhdljn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uptelgww.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2krmpxyfq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kjglkzoz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sgkepjcx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ahcwlrrh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ebkwrjlz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ypccpfqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zqsbcdpn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2baomcwnr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qhogmjbm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2goeuweyx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xfrcvhgj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zeterkjj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2oooxmjjn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wuvxeuto.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qjlbhjdc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lwtkwxcr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mhgghcjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pcdggfup.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vfnlwrbt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2poigxdgz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ioxcoppt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ffoimsbe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ptsdirws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bhvnqyqd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xvlrtbhx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pbcvrjqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qblmqvnt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2txzxkujl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rmhfpqmi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2atfpally.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qovyfuia.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2okqrzmqu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wibqkxvw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dvofipsn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2huccjrfv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dierutke.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eeocpggy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ovpqibof.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2guqapdlh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mitmogfb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gkifmlwf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wtwkuebf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxqzvoyf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gnwmwndm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2riergshl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2glzgkiae.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2osglkoej.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2abwpgjlm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2yacfakph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wuvtefiw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wgzqrwfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ggbyywdd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lvhngbtc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ltdfftil.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hqekphcs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oaywxogf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cjlglxte.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2llqoymft.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dhnklmba.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2chdrybyq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eelekwiy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gkxxoztb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hnaicvkw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gebkfzzk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ietuqjwa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2revkuqda.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sunprlxn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jzpyytdu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2twxjjrpp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hgoftgdt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mdfovsix.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2buzewmlo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2irxslwvr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijykzrre.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuouiwgb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pcitgvmn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pjjnfdfd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vwmvrttu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2aoituwsj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2anutrwmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fabxhmww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wftldzdq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ojngcaqa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2amfdaoha.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wxpilfne.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nqtbldgc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qitkmvxo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gtyfkdyn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iyfphory.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gtmkfrzz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2scgwcjhz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aucxkiyh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vdzvzcla.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scdqrmcn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2evmljcfb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrzwnqv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zfbmtvsv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2erjtrnte.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zsujcwut.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njpfnuar.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vfrhczfj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ozrpilkb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rtiqngqq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qenmndwl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fuotwynb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zsfdcjzd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uinukpel.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ofvqimmk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cexumnld.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wcklxhjx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hpdreubg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mnhaaker.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nqwdhhzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sacobgfr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wsvamnah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaymqoge.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lqvnschp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2numajvrr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2luhqnmgn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mqlkjvqw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uyzdfcbz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkbkqryh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wvvmqrwy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgdqglkm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xmdsjjnj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nhqzyljz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnnrflll.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2olkuwzuh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rwpdyrvp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qfipqgtt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eltessdu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbawotxf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vrndnvon.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kdccwbko.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cdtxgkip.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kfpcifea.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dbyglogr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fgbdvuhu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2azfdkdpu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jixxdwmy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2labbddin.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nxqimboh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2elxnomte.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezoisokl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2efeprjzg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2huvtwdel.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oqmdbgvl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jwklcpxd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2elgwerxu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vbzoxvis.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xotiiylp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xojgjlyt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2omwbkmhx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aazxthdr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dvauzjwe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dscvztwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pupeoaip.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2etbuvfld.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tergttiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2iawmslhw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lvglhycl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2igimcvtg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuiyuhvq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bepjtofu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2iapqweee.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ysmbwsma.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ttrzwllc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vmbwvhdn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dbdlpjys.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2oyuosuog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2wueiuiwm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uxhlbekc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2boanfwpc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zxxxpmec.html


<!-- 参考信息 -->