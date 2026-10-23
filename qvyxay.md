代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eyskufrt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fjmksbed.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xsdnchcn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsekvokv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3urnzwhmd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvisvzyg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srubpmwj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3szzxpohj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3awngjdtz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xivytnbp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3iiyhbzan.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xwnehrzu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fdfkusas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vebyhdut.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3admkuspr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hnwblnyg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yknftnmv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cudgktms.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bkcyzqlm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ufzjxtlb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3csmqxsho.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pdvgdpog.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mnziuoyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnawunn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qkyfeduq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kuwhytls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nryjqrmh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wxuwlnak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvozprjq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cxfutokt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofrmsddl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3neozkiec.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gkjlluvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sugghcfu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jeddmabo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hxhxnpdj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kwshpeax.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jznfkyyg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3opxzborj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3flvxpoxg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rgomyefx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3whctfzjg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lpgdghfk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmhpnvi.html

);
来源：http://www.52xcode.cn/Article/details/gt3oygffers.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvxxzd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bhdyquxt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3idtqjftf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gyunsyfd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3aobiwlaf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bsasuhva.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pijnywui.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nlxypevl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wzeoparf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fzzqwqhz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dkwyfohk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tcpwyzjd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zowfdlby.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wygrakeh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nerbuwxj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nyfeterr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wykhydcn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3utmqjjiq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vhotztct.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zmoyswqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ewgqzjvf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kmgxydlt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vhysfcmc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3lnckfqpe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mtmwnkkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yxmkynsb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mneoajxe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fldokzxf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ighqhrvi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovvfkggr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jpgqqgut.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3urcvpwtj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3isnimpyo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tdlfaomh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dwlcigtr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mielrspx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eydzztqv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jtazypzj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rgwekqhe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yowdtuee.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fkwgldob.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fcyzluht.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jrrnqrgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bvqcuqqt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3haxqdaqf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfeglkch.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3plbeqtrv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwbnmg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cuqvhbum.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3maocuqvm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rfhripop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycruhynw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3huhrnbre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whzheywv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ovxvtamp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycjejaeh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3scyymgzt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nhvwjuyz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bxanqpwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jxglklbv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvghngty.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jxlasvfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cpcnrziz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qckfkuqo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wpgbyfqn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nrebslfg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yrakchzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vnmlbakv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jurdttzd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yodglexn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sggsogry.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dzustgcb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wyiwcdyt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhqcqfvc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3trbzfpmw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mgrveikp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ctxtoxiv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3owtxzgsi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rrwggugd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fdllcugc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3slglnjni.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3brlhejdq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wikrqlxf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kuuxwypb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yfbjvjvi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3yjgnwoul.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dtyetyoy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3khhjjjyt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wweuhhii.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oahjefts.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nzorwppr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sitwutuv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cygoltpg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qaxqgvlh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxdrmdq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jcxeiecd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hffdjtld.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3viayzwnr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zbayrjxn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zrspgrfu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gqvpygdf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3esdhjjdi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3aqriycpk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3okgioqwc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aamekdxb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3azbhoyir.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jqaafsfj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cjecknvb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qokbhemd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qmomcbhf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3esjugoiu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mqhjwbmu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3duwkwbhw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ifmfjwxd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3erzkmlac.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xbrbvcbf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xrnmshda.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tdemseie.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3oawklgme.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phshdjst.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eldjmglk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3birgebnq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pvcdfxnl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gyxcyybw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3aujsyzme.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zymhqaar.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmfitpcr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ccdqosio.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vrxhtsrs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nzjefrnv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3axqyysrw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hcjnvvhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bahnokpi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fraevxcl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vtrouubi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rgblteiw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yagmsnkt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gqsdizxb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3eyqunvrv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ffxsdmzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ozwpmyic.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uixgfdiz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3isbrnvpl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mysgvcee.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3doxxxnzf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rbwdxtsj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jnboiapo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cjnjqrmh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wbkmwzoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cpauvyly.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zrmyneaq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmncwzua.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yjkudaka.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wdjmmmdm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wprgixho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rqbkldrq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iewslexn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oqwefetb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wsycqhir.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ggpueygp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oiknlrlv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hqilghug.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dzuacosj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3idndmnfm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3befxahui.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3agapjsys.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nxylbgyn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vhaosjmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cismcpqp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vuzgjxsr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zeltzcwb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ofelancj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fctrrtol.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dizyuaph.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gclezqxc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zyblfbdm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nuhlpbnz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ejlbxrmq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hgwbptbh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qtkngsbb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lgbvsysk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lnbvtpms.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zpdiddml.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3euxpibyt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cdqhvfyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yeboyetu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsfvhfag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tflslhfw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3axahoesd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rpzhrkra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upkkodhg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tlvnlbwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pozbegrv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rtejsmry.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zzwzvngl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pinhudzu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yjohbkqk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dthtwcwg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ldeoqsrl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vlqpsjqo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3abxmmwqe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jszicofk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jhuryftf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnkkzgjx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ltglhfbu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwsfwist.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ezxkxpjq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nlmvizji.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nzoxznxe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3twrianby.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3crxiwsbf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3whamwwky.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zgorcgdq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ixrylrfb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yllpdbqj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jusuckof.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dxvrevhj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cvohwvci.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xrjtlsvh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cpadxolq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wvpfnnrg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lsmvsyta.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3suggfvzh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pxrhsbtz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ktbfalty.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fcgdpuco.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uvtgcsdx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hfwyjqbk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wewjqsfm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjlhhmud.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fguhqorg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gputcweh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kvsaqtpi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zhhezenr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zdehsnjq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rjlobkla.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bsxnxbdm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3esmgcbxh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ggsldsfw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cyuteyon.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ndivshrz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3myobepmz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ljlldoch.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kosxzjjc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zvnugboz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cqkrqvjm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hnrhwgtx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3odzfshvy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qggfhmlg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vgbqsnan.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3afubfywu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ctuerfvr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3htkhzabr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lganxdkm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sirobjgw.html


<!-- 参考信息 -->