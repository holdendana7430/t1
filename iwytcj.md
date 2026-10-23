代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3loskshht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qjsvdwcn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtkixr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lgrhsvdc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3frxpkjgl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lnewwemn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gsobqnff.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3txzezrxe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wxgqjmef.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ajkfjenk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xhuzksad.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rfnnhbna.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uwaabqxv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rbxieypg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rytifudt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zmbemiiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3takfdwgn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kujichgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kldusnar.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kartjsgm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vjbcrumq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xtqxcxeo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pvsfzdyp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fmjwvafv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bqgyijwi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ziikehkt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kyakgrnh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgtwcq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qrnzhbrx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pkkfnrmp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ekqizzgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtnptcv.html

);
来源：http://www.52xcode.cn/Article/details/gt3ekemwraf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dyulyxua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ltaatdzm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hxeykjdp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cnbnsjnl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3navyyuch.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmdphim.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dmzstpdb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jlivsgvh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bbjdqtru.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ocxmhpps.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3omfnpjul.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ufbqmbmk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cxmeaayn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jfngdvwu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dauzbmkq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vrqwlzta.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vqmgksec.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pfgdcwdu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kyycaewy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ryullczq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lpmflada.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vfunuwrr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ebjhjrcn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vzerebkg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qbboavbp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yiuoisfq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bfepwxgf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuaqtnxr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcddtr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3quzhynyo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jttaucxs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3shsxqcwv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wjtenogy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3supvsmmw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ipnfrmdp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ykuodchs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rsqhqipn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wtsvjvka.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3byepccje.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bzvjpgth.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3newjaels.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tkklchan.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kdyqlbfe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3krvtrbaa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qazpmstw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3odlwfyfp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dajnvwda.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3novijmax.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ihmawodx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eotaehox.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lrpklvuw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfkoswqw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gmuifgcq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lrrqlzfy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cnoetqkz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzcjcrfk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ljhpqifz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cedixtwe.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3veceidyg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bnrihtyi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drhzydid.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3glnysdws.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3urbenlwt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3byeqnxov.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ifpojais.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vyauudwj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pryjdkwr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ejhvadns.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqwdqxb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ucaswswt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3emichyvz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3iroxlval.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qetneijs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3clzfxjvj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hirvvaxd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fghonces.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qsrfibde.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3phqsjeca.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rsbyrfcj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3amhiofdp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nopxhcop.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rywoafjh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3syxkhubf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zsjskpij.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xdfkceop.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uhchidfw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogavotqi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ozkznpzu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kpitxqus.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wsehedkw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3aimluenh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ndxytfkz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3udtzzefb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vypynpwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kkongxmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xivgyyhh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3izqilpej.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3uzjvftvg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3awqotmup.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bntgtpsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cviclydj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gxtjmmdg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rqitjwqo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fjtexvlw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bdqqzedx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gfarzpqy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bzcknclz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbelzrwk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cfihvuhf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bahueexj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yxplqtlm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3utgrpvpl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3edyejnea.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3phgyvmkt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qottzkag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jysqgnvt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jvblaoks.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kxcdajek.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pzozlffg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjgmuhdm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nlhpsbfc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3reuxzazj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3veijypyo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zrypvaoz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3orgcwcjr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rufydjre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yhpzladj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bzcifuxf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3omvteoqn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ihrmgwqp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hkdcbvss.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxkakh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cfkvebaz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mplodhdv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hljbsqji.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtfyojnu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ahbngkqn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uqyonldk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ygynhmgy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yjcmcsxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cijypead.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tcorlbpo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdfiuevx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucnffrvx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3djomqoxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rlhhiutc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3typbtrmi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ceanfgwe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dwwttedc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qjmsgxyp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nnffflzs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dagaettt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cfyilunj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hcqbewlb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mygqlnbn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uzbwsdgk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwhdunuw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3afaybmqu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kytpalkx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3onyqgwfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3oeblnqrl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zwfjxnga.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3uazjwnkr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ifbyrzvp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dteljgdi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lbfzvkdj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mmtnpljv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nmxkfzjn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hczidzpi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pnstaunv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utygybmc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pobpzcjx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3haqcsipi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rmmfqzfb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzcbdizw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3puaponaf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojxjvgdz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vteuhywt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mxcicjhj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3klciweng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vtelvvqw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rlzrhkuq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dtpyjhpr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kptlydzk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qnroreqg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qabeztju.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rlmweafv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3avtvgsxd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wtalquyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ficgeenk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zycbzpfz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sksryemh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzqrnmtb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3npyjasjz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ghrobztl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ukcposas.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3txgyywpn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3keuuhvol.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qfdwxrxb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ovtfeaga.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3baokdhyk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wcahdjvr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vplsevwz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3imqwrhgn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vmidopgg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eofquknf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qdqhjrdl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rwpwqpoo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3djgcwthh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3rlorevnv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qhnfvpie.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3csuohota.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tyyjmnbe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vsgzqegm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rwmoakxe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ritldwfm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ffhzycuf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xybzigpp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qcsxiyhn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3azuqynmk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cquklkcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tpcyqrpk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3illalycn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wfzlwdqg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ywfwgioi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tgzwyrys.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipmilodx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hvjrzntl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bjftpnnm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aeaxkcsv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xdaepjes.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3klbfaecb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tfuawrrt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vblpzbzf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gxdxkeqw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3acoqmybh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tschghgu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnbctvss.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fimzuvcv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3exmwkvws.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hajhtzfr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qpqzzzys.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cwkqblpo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zvtwayog.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fgrhagvs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tjydgbqg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bedmkhwi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xombilth.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3plrjszpr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zisaqudr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qtowczmj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3havobsrm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mspqetex.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bakvqjgg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouqgdirv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nsctfqhb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3affitqta.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jziebqcq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxpwfpcd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eofwfnmr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ofakbhgf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xrciacfn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3buhjdcjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tdiyfhif.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3imyohzes.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iqsaqaki.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oujienec.html


<!-- 参考信息 -->