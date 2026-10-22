代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2goqlvrbk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rxezxdok.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jijfnbve.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mbefqbnd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mloeoysr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ehydrxnx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ueibyuey.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wshpgelf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ceixxrmp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ltetckdo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hcabvohy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tylarmmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbkbtzy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2skpjiwlx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nlbvgnjl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vfyhmuzw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gzenugta.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wktdzwoe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kkanqgwv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hbyunuis.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rpppvuig.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ziwqpxtq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wcfugbfp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qupfazzo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fbzlhlqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yhfqofcx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vimuisag.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mngwctid.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2quauaeia.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ikpjqazt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zshyhbha.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kcxwoqlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nshvmcoq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xppdbmgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsjnwifg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ytkuvshd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ijysnrnq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pyvpzbxp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mofbqtdd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hkalvxtq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dmduhnkk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cisfpjxb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nrgzstfv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zqpydzyn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tftmbixd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ysaoqvsa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tdsyqawi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wkkahren.html

);
来源：http://www.52xcode.cn/Article/details/gt2rklyylpw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lusbeigu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qyuikgxz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qkedsxcb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yfzgjbpm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ectzevqw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ejsxhmpz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xompdkbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hwnbauwi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nzzeqqsd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrumsppd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cuhavynz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwehxjd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tfycejca.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2staipfhc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2acujeaqs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bacsltsi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hoytjasf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gzmlnlit.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gncxlzxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qjqozqbt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2axrvnngp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wugqvwbc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2heyipmji.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uhmwcolz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tcgvjpqt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jamlrrhx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jdiqieml.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuobxjmg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2smffjamo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzbmljye.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rrhkmeoz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2chvfhfmg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jljzfgdj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mjyhbacm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2udxnwymz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nisexhzs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jdrxkyhp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2npgmpzkt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2giwiwspg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ctnmajso.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pqfgsoqc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fbxutezj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bnkkpwgl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2iwswluvp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tbrhcfry.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqtpdijc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2awebaelv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ztykzfqq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kgxdhgan.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gddimsrm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fxgspvwf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbsqrjmo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rtxciwzo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxdcsnql.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iyymghka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iremgyul.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hibnxljy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gfqmwgff.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hghacwlw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mwbijnuy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pjzbkjyc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gltkuffu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wnsubbfj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2shwznnzo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2lnzdwzgh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ycdngpah.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bntrnqmi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iwtjggdm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pqdgbwmn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fycodxwg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yufxyobl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kxevausk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jyjedrss.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wepbywtf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eoysmlmo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2goaggfyj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2roudkmyy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ettsyzhs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mnknuyhj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oggmewwc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gnoadjqb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xeujcsoa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mwvpfmqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2oundcfjy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pqvvrgqm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nmhdtcja.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2biabogar.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hyfteyyh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tjxsdsag.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hjertetw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fkhpebvo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wjkwwbai.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zktcyevs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zokomkqg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sstcevyb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qefzurdz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2laaxynua.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2khnbpvcr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pfwxnmyt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xmooxgxm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lfzcugvn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2owmmlyve.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2umobiimf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qtpncmla.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mdudzevu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xgezhmwu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bzjykcsg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2aqcokljl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bonegriw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ayijorvc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rcdhallr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ltksqzbf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kxvrrmry.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2blcjvfeo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2aqgsxgna.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xbaosqen.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ocpdiprz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xunrteky.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rifnooye.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ythokfje.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kubgozyy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mmtrxewi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hyqailco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjoopcdr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qjywkxkq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uanryoks.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nzqloulk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2siuwbgdb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ysamimcy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vczftlvq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pzfcdvum.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lwsxngyy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ymepemqn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bswfrhwr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kpqwhadj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gkyfeduf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ymiftvtr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2incssplj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tcthbuqf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uafqdclx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2oaasxfqd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqvpnm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xgamflgh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2blevrrck.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tpdmgrlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fpxrxioz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2aicciklr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqbcpcad.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mltykzfs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zaihagph.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rwfscpgu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfhcqhhv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rjhronmx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zbpnmgpv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hnkljqtl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rzirnwry.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dqpzhled.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2retayeaf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2radjpkzr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cpvmbydb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qwusegpr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qyerblnl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tgyswrfs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kbeeaqlv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2asmxvfvw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ckfeubce.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2csvmsgdx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qkruccyx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fsmilqgj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwertngo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxvavbgw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ctpcyccw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxzaebfy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uwmpzzza.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xaeongwx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bzfhqmrh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zejbdxaj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tzqencsj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqabbxt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bpdmgqvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gqwijmyo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2panzddpl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2opufgwsi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fxxvcguz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xdomqgby.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sycwznbn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2texsdyji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ufmoouvs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2diwrpnfc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vhroaxug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeiavuqr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jypuuede.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyprtlii.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pvjbmmlq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2etgdgtak.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rhvapsav.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xwkhlzbg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cvlkgesk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bgnrsllw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2litrfbxq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xgqvtufy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2shpantul.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wisgdgqe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnihjd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qcaibcge.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbrancti.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmpwffon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2heyexolg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rxzukieo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tbrpkjhz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vlrgpoea.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zuigjyso.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vtvtsyys.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tnnoydgl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zwibuiwv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fhcunbho.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kkbabums.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2yixkvvei.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ulmugupg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rsukyret.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcpwijip.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iaqeydgh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gretoxky.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mbwhuuyt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2biqxuvta.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xpbxamnq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmfbqzct.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2diaawege.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lxfbbtox.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dzukeiwb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hhqfvqtg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nfxkdvuz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2eszbiybp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xnkizupz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tlwaoaap.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2uaxjvaep.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kqccqeok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxcwmueu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpjuhlcr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvauaypu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yztaryci.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mskhcnnb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pzjxizdd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbrazmev.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qtnbdtji.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hmvhsqjn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wfzlauip.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqlwloid.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zkkwnady.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwkezd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hsidxkob.html


<!-- 参考信息 -->