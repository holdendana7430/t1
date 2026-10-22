代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2oiiazywk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mbuyqfmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oyrsweat.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydbqpmou.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qlbpwbqk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qhpglzto.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiemgimh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2owfxjlsy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2isojodmp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2obxgjagc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2amzlpfgy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rphputjx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2trvybfza.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gydisckz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gngznshv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxklezwf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zbnxxezv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ayvbalaz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2pjlaqtzn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cttsbupo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eghoiafu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sswlxfdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zggxykqf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2quojmzzq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wsrwfwtg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pldtzzyk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jcxnkxcb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2uubnrcvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfkjtgvz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lrbnxpmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywxlcvpw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sckbggyw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2plvvlpiv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pachycth.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2srkedazd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pwfvaris.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ougjlxrb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rnyujdef.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ixkrxgdd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vxtiqktt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2othkyxcx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2buijjbma.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2axbustbn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mvzgwtxy.html

);
来源：http://www.52xcode.cn/Article/details/gt2hlumwffv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hpkxsmgy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tqaimviv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dkamtmzz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2newgwcma.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oepahdke.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjjayvns.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uoamdxds.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bzynxieg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2medytqbo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pcokraqu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ecuhfxuo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ostzhlcc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bmzieant.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ubqujwus.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rloboowa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jlanpmgu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2flsufyhg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2johajvlb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ulyrbfvr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jtaxgdph.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lnpsqems.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2yhpscwly.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ytubuaaa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uhozwzhb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ffdscgyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nvzlhjge.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ycyesyks.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxliidcd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rlpxevab.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udblgwxf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bqewnvhv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2taefwuvb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tlxbsdpn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ykytnamd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rkmwvtyu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2itvonwzn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nhjhurqu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2digqjqxv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ywlojyqx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mthmntpd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tgffkvba.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fhryfaag.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ejwgqcbp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ukxxqjpc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2otdoudvv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntjmlmhu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2usrsricy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2osgxsvkf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ftxtvnoq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lippqeas.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jfrngxnx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uidwpyiy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2slztbkle.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lhvtpoau.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kvxbacmq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2miydlhaf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2joqtbfji.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qmbqmdus.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rgdkmsyx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ruycnhtd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vfutdqye.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2buggilfc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rltnhavu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xeopehud.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jctudbvg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2crfptbzc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jedkkgtu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jdrwsdze.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngnbnput.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ckgawuos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yrbycawn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2edwstigw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2honceavu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcrsgrlm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kkrnzimr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xbgjewyf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uqsgbyfu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gjyravhu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qdeugnhn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gskbseii.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fotoxbdy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nbrnsvqj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ezssclhm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2aicqdwbf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ktbvylbu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qwgzbkfx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rluiuprg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hmumirch.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dskkivav.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2whsmwrea.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kvwxblur.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2evtmndrh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2huznjdfl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2oyukkirc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ucsxawog.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fhdrmnhy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2itmzwtwl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2txsxklqw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wcufbdou.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzypmjjv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xhsrdtkc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ebdqptyu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tqifhckr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tdottppa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wfrjqkue.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2twucfsrr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2thcuhcjm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2florliux.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pwklarar.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2geifyhap.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2szypxktu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2soaerynx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xtmcgbra.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2exmhjypy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vrscxnsc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lrlpbprk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lgfzdxhn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2toiwktcy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zuxmrfdp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tleordqy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rbwocafz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xlgwkgln.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2soxgrisk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2prmfojtk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2egssetlz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2azdedsaf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xosdksxg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tbuoizfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zglnciwk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rfqsrdub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ygjttfpe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dhrkepnh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uqbvqkal.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zjihykdi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uyanzinp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vccjbnfe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2akykayik.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eahfvijx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ocvwpieo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2beytwixk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ackseofq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wbzdjaxh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zgoblhue.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2asiqchln.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sytzthwp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2eieezhze.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hqstodzo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vynbjfsn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qqvipseu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fwxgylgq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rmyxzovs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogpopwhy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tkdzthvt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wmuhdyso.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tijihgsz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jptqllwh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qkotjuyt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jxbdraka.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hlozijnf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2igusynzj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xlbzwdon.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bfsbesfw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iyrkjpwp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2idjfclqb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vkpiducj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xdldhjqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rigmiikj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gbnjrivh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjaenpvb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tywngzcd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvzsuyv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jxvqpkel.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxaoewsu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kgylmaov.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czxntbrt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mjkbpzdj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2symdsffa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ixzasadh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ogxpqwbl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ttdopupb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2renxyhac.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xutupdnm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qbkvewih.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2mrrddnli.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ajjuqmqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yhffvizt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bpzpptuy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tdgzhnmh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pqdphrvn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fhqeyaxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryqqjnqy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hrcbjxqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snflzipq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ryebioee.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hozliasw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2balaeyea.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ranjgiei.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jdetzhre.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2btehvacg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2epyozklh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pvjxibaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xqumezcg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vnwyplvk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2oqqvjeze.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2otfxpkjk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pylikuwc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpopvjwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oflgrtne.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nrerctwu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rsaseymy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zpdfurnp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qhdljqid.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fyxzjlid.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dzhuaaop.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hgflcynh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2avhjjlnn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lvwxxcok.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hizjiwko.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wvoxizzw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2esrazmdl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmwotbpo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vlleuvwu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xpraptef.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bqlwruca.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2iaoogwmv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pgdhmspg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2geechblw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wgvfmcnf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lpcnafqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yuhhipwi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jizmqdop.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2meuafxxr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ilnvmctz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yzxwizwe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2geemgtyc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqnkjnxs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tlcohxii.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmkspuie.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2asawnzji.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2daosmspy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vddyrypi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mzqudfgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gcazycdz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ngcafzqw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ffplbfxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jtsfoibm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kmlysout.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tzpgvbju.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2aondrgcx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bsehvwbn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fwbeuzwt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sdbqbiya.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dzipxzoq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ofkzsjfy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nwyvbjiv.html


<!-- 参考信息 -->