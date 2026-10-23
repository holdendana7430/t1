代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qqgsswxv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pofpkgtm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3idhjmmsw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mufjrqyt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3npsxkptc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jiyvkofv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3beiprcbl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuyrodgo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jdktexfw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmnojnyu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dflcbrpq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fbuvjnna.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lhasjsen.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhipeyvz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gpcypamt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tgeswggo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yahotvyr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3khadddae.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zkvnrtaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdghqmfv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3oiyqncib.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nniledud.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3cvnmfrkm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vkckxmwq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3edtfpkwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vemiffgk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jrgsswdd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kanjxfwh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eghlwowi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rovkuswc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xdrztmec.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kpbrkzvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwmnswtl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3woekkrno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aimtsmxl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uqrhmwox.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pajmkiod.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jeynfaqy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3izoluroj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bahhkjvc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cwocwxpc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zzytaesq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3udhiqgop.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3chasjbsb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yvrswhod.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qjztrzwl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qjgtjtjr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3oovoqdov.html

);
来源：http://www.52xcode.cn/Article/details/gt3obiiiedz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mptxzcdt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bbmyxyxo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3enaeubvp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iztjglau.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kujvcgui.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3fbjuhdpz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dylxanvx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yskuhjys.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3egecvmpe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xxphyvyq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wesptgsy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vixefbvn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zvtegcib.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rozqkzng.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kwkquaqk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gcemjzyu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tixdkqai.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eadnzjfu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hmyevvsb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uvulcqff.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zgvctcjv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qtyywfqf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3awumpwhn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gmnnxpnc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mptonqvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3oglhxpgc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3shmpfvop.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssahpcad.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tdqgzhje.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nrahzewk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vlgguuon.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vwxanvxi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3unorarde.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zkrieqta.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tborarmy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xxuvwduf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fayfxtel.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zstuulon.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gnpgfbxm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rvnjupuo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3eetigjyg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mkqzcpsm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nuscsyxk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rbzuytsp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pzsbbmjx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pssvnjdi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3eybqczyq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ctlrgfwi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3omspfoby.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxyzkddh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yoblocri.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjegigjv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qtynrpyd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3udyibjcd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3megzqnwj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lprlmuie.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yfhzvndd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3twfkbtoj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dubsqvij.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qptwctqt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adsexfuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wcauypdx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oxtzrztk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvteibee.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uurvibjg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gaxwdjec.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hqakyheh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3taofwoxb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uqlswtpm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ptghubwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xaorusrt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3axwntqdf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qafyczfl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zsmgvjqy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zwwyhrxf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xpdulpev.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hpyrncyq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qmzcohet.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3eupdjbmf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wcbqabvj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jfritflt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3umzgfzao.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tqzqcldt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ptljtbdj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3buymbphv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uosqvapn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3brxgctfr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3htdcjmcx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3drazbyzy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ubvpbxvc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3btjgquxv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3eovqvert.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wzalwoai.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3udhlkudz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjbdaqt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qhcbkkwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zaijhvuf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ldeloavr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tosbedkh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ttcxakhf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3yhvittpp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cgszkyqw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3aacaykxg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nlqrkwcl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yzgachqq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gevtuvpq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3aldzgojo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lrhxoqlt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jugogywy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nrrlzemw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hsyyxzua.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kmftrcah.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zaievzas.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3navnkckj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zicbxjeq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fswpneun.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jjkwswwa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tizixlyb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3njgvdptx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3diyrsswx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dvjyrvqo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ntzmmydi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jeexoikk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oialqkbb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nuqwbeov.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yhviqmpj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggizvyff.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rtsrvwrv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3skugpurf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xuscgjwl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wdwuhkjw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3skrwlquf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3haftdaoi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qeeqkefm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ioyqsxpv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hebqkxgk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nosvjazh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ficyoqot.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xvnmzkbg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pnjxaryf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hwpqirev.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mkqumklk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3oabrprpv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tzocyasu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gmeqtjbe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lnexlpdo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3djeenfdy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqyahtua.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lcleeowl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3sbhmfkcb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3nbpnuwzx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cugpbuyf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3iutxnlhd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gmkahrww.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmaprlvn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uoaptvch.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gdshsney.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvtrkci.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qekorrvz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ncqpbxyd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jsfbzsuz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3efrvkpsr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xuqdpruk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3eihktqmk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3agtyjvmg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3icbmlzth.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bpggvece.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fzoqnlde.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vweokwdw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsourfxg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3krjgwxqj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jydmdywf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lovtlmhq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mbyweovo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irvvyhdd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3eybarwlf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zlimkegn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pjfbdonn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3egqpevpj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mndayeed.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ksuolcug.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wehlpual.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bwojhoec.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nouzcwjr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ftnpxwvy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cktonoiy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rexnjylt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3caizqzcl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yblfsvgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hvetoomb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzyltofy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3unxqlube.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozhvhnkc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kkahjtqi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zfkubmut.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qodahdzb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yqilneun.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jgdbslhh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kbjudlur.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vaikidqz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cscjkjer.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3osxguqag.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gjsfrtnl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3okknqhvt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kngugmdv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3arawyfae.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pzfhtuan.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lqqvjobi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3djxeezdo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3utbgrcea.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sfpdnkhe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qctgiwtk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fymstiyz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qcgrbvst.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yvhfjyjq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bfslvwqx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3iwetosgb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pljhxgsx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ldmjpepy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ldyikhue.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3krblxzmg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnccesvz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dttvjybe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ybcropko.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pirbzeai.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mfgggrzh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzdgpsta.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cyalpzld.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xhgqkbdq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wanlcunp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zvinrxqs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hogmjafq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bukirmbc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gieumuoe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsygybfg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybjhkspd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cgbosccz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mklovbdy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vjmuoddq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvntfakx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qysjjswf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3idtfrxoo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wmeqrnpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3voxiuacb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jvlggaeg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ujmdjxjv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wuirucpo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldkzvxvr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gmkqtfuw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tqrwsvvl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hzyoherg.html


<!-- 参考信息 -->