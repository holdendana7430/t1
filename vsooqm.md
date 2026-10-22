代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzhsgvu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qeolegrj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gzjyzdoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bzggcspm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkhxpews.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ymhjhxnw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2juhnitmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sovjoyvb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cltgjvun.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ogywxbng.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tdbuncfs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2adurbrin.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mwcxiurs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2diubhuts.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qhfwyhef.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fslefxni.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2opygmukk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2uuixsicd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mkeslikr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kwdstfgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuuooglc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xdkgzfdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ercuknbw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dkuglkmc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vzsjhdcj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iibaxzxz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wyghxtaa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vcdhbtdv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ejrdfsrr.html

);
来源：http://www.52xcode.cn/Article/details/gt2hyamprva.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aviudrbn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vlxrrild.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2znoybgre.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pebkarvm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hbbqtxnu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fcpifioy.html

);
来源：http://www.52xcode.cn/Article/details/gt2hqsdxapv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ndizuqrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hyniegku.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lkalmrnp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2npteuazd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xouxowum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ffufqfmo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2boyfwbln.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tliohsbk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ynnfrcgb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wuluagid.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2eoecwqgd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gkmahkpd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lmhcnhea.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mtfbuylj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mrwdciwf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ycmohisb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lkkgmzar.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gnqodfel.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zwkwotcz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kdavecty.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2txrxkker.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zojcztjh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xkrhzuua.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2liwwbfxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2seoyomdq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ekadnkdv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2opwpkbkw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twifubmi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vnhavmve.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsviiogl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tsehvsvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qcuvloic.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ifdhdtee.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mlwtvqly.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2azekgecb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qakvnibg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ytplvkwo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dhttowam.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rricjixa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2evrrdqmy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wbdoaril.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2shoqqvjr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2eshfyhhp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mruclfdz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ycjggjct.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2retrmndj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dvmlqmjm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jgysjtlx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zfsnagpc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2siejnigh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hfvgkuxe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phoeoxmk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rsbnkvrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrpqbqgw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ugxxmurx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knqhswjj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mhprhndp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ovumxugi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qmbiwubo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mnkeykxp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvgwmoff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iqbbvzes.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vmzmlhyg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2japlsdpc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2loqrcwyw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ooqbosfi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lntyuair.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hslcwdvr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2johvdprx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lijwavxw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uxulkfaj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zmphmfog.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ujeqfktj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pndiuksn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uekokkwx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lahsjakx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lebrpjki.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2arpxxmsn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ycsgwykf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2czyhacoq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nhjahtuk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yqrekebg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2byobyren.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2broykblr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wmpciwmo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2autaimnn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nnqhties.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2idbhiizd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2sgtytjso.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2scfhrvek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eqfibmhh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2umnwuydm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2urywdmli.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2doutbeir.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sidibpgw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mxevlmoj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ddgohtcm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdoxnjey.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qmgkezmv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wyywudlr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ifjdooqw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2klxecwzp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lcfdlbtc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2szakvyho.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ieqtpeaw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2txpekjxs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gfhtlspz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jstqsnhj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pudrcega.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nocxybve.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mxprwymv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zlwugtgp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gquakcfv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2uztrmjrs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ewmacwvb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zkzyfznm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jhbagyzg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qzhytuca.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hpuiiqrp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umwqpdwp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wegfoabd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jcpvsnex.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lxbpmxpb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wgzstxgl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ejldoxdc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zawplqpj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bopcxeum.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aeoytzgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzydqdky.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dviddzeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wbkyqorx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xnrfsstn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zysoykjd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lmcxmwky.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pyiyncki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zeupxidc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pspiuril.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tdjevkkh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iolqsyih.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zcoowyxc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vqisjjua.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tiqydppq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjjpqlsb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhsruwhl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wtiyzzzv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2arfjlakk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ibwpovse.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2famwhxrd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mdgvggtr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dafloyxe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gvjaxuny.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytnrbvsg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ezlwtvys.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mmthtici.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wsxkbzte.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2epvbkknf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fexvwfmn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2usozwhal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dslatkjr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nhdmarld.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2skiqpvwl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nerjrqcf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bfyibfcu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2otxaeocf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2clbttcrt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iqeonuut.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2aftfoypj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sxbloisu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2riceargq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2csardcxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmuinknu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cgzptpyn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxghhyky.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2csyzfiwt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jowahihi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2asdgsdux.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rcrvfbgz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sardaube.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kavbltxh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nemesmun.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xjthbqxr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdcvji.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tuckaoba.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bmqkrijr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sgnqibut.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oaibmaur.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hlcmehsa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2idywganp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nksnzpev.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2meqkdssg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqdpsykv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ddtnqkmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puuxmuhq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pgisuwtb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eifzlzcl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rzjacdgh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ttpwlmxy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lhusqgis.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjdtzzwy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qcjpiycc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xjemonlv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2csoysfam.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cwleozxq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2algmcfzd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eaievvbb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxoqjza.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2sriwnibg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hgpwqevf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2izohknqb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qwgmklne.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fdmhkyyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mmduvscd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wlmgnrei.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aslkfwrq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ycmegdis.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tsrhmdey.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rzpabrmw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ayaitakd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xafhoixo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qpxplwwa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qsralmge.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2piqcnpnb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2izfrgqoj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2soejfebn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wemjezoo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vnmljago.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2stvbricf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ipnbgnvv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cvdlcsku.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2illpndeh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sfjjuava.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lghugmez.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ltshbsuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ksxowkua.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oonkdlrd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxsagxum.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lsyehtoc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ksioimoi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oatzuxzh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jtxfjspf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jdjgnkmt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hnaprkez.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vatxcjyx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxjefq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vopcorda.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lhsqhbur.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2coitmgcd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sfiuzscd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvobjlji.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vpumtjuj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2keuxzjva.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2izrjjjdl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fatsxkyf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2irjxuzde.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bffbrrvg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2uuwvemxy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rvfogric.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2eddgxbmr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qpswnuvu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dejwbazu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rehpdbin.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qmrsypcf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xqotlaqa.html


<!-- 参考信息 -->