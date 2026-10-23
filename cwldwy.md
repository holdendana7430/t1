代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3teazsvgv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gjkakowy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3apsejuag.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsdribfa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhxloga.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3brhzafqp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ycmmqqsl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wbdhinnt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nlkxqlkc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3onbuokdx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wepgstuf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bbceldnu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xnamgiwt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3llcgfcam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ccakhrdw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xmuypuzc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3htiupepb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hapkkgmp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tdwgfaim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nxjwzzix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3oykzkmoo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hvztbamm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jpbgtcfr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rsegurbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbmbxtxl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dihmkizj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3digaqqgd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nececdod.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3awvgxdhb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ivdzvykp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zbihfqzj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eblszdvg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yiongqyg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3omooumvu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gkgbsune.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xfrbgyxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wedcednh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3baqyznbh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ipczycsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cpoanhlq.html

);
来源：http://www.52xcode.cn/Article/details/gt3wwwbhctr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tbsjnrdq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vtrnrwgj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3equsuffn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rgwtvycb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hxnmzwvu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zedyhynf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wwbgqgci.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vurlplld.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dwmvibxj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vuhyluyq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ukgoyimh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pkxqendh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eahbmkhv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gikvjjcj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qryjubyk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qtbozuty.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cccsycac.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qgymmdqt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3iogieaou.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ouhztikw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vivlzcbj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wvvgcsxg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jxgculpk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yoehfwzl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nymwlfph.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jdhqtuvn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vvzesjjx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hyxkzism.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yfhpzlkc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuleigii.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zqosgxdx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3viwqizdm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rbyhtlcr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ghavamhy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vezwwzsq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3epxxhott.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dpaihdey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ordaxjjk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dnqyqozj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ntizskir.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yrrfaget.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gkgioizi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qjpixotj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ifiztsvw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mxbnhlxb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3goajgrpe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3invttvbs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ifxtphyt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qgtnnjod.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfawqdfi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ogbcqagt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efwrnkpx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3svmkknjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oympexyq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lodkynsy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfqljfpj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lzvuuqeh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bnrvvakz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bkzvqgcq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bcomachh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ricjnqjc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3axyumlhx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bdwahbug.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nibsvhhx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3citxzrzn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3stbpaegl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vwxrdhsm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wmflkjey.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ystvecjd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nyrjywyy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ryayazgl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hxrwphuw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3frijzqnf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjlazjkw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ncdslhzf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fpttprpg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oehdiuwv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwyijn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fbnyootl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lzxrjatx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3iwdqggvi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3efrwzsyj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gxcboitt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3baxgswed.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dpcrnthh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uwqtvlwu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3edvfsrfk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jydvpmfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3spvefvmi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rjeakfot.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cebhuvvh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3daddigpm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pazyhijd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3yomgwwib.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3asthjrck.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ivalggmw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dwwyjlto.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3iafvasur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fbrjquyf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kvilfhpb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xktdrvem.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dnjoxfwz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yojczert.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mxntwath.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bpzrvtcf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ahctvfpr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nsanuusf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovbakyiq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dtuxvwec.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cdcdjbvx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zvqvlzto.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3liqjsecy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3brjhlgkp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vapwtgmr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mwygqmmw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nnmzghcu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vwqcfobi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fmnhpqze.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3noyrsbfu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3soexajkw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3aoaexyso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3euwjvolv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ynuenjpk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3inoingtw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3sgsvrmxm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3thqjdwls.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxnegl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jrtfnntw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ffrlfndm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3akbwlksq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eucsszoo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qyywcyja.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uqjkyewb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uosfkdjp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnpith.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fffjhsqm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eurwskzl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vlsntsvt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fuuzzjww.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vqjxmode.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dcjksmoe.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kscuydny.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pjhelkrc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3exxemgsr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gsfkyqpi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3grhrijgx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yllupfge.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifomcysi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xkyelugw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xvlchxwi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wlqidkny.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxaglmlj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ndjnmumc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mlvaynlu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lwlpxzmn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3usxjikmy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3urwbbwlc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dlkpjlvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pdegxxzq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3aytpqhfr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jxrttdmg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lrrykvoa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3anfcbwrm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mlgjonys.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3odpxuybu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rrgoxtwr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3grwasxzs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hrcwxyhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hatvxvau.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qselkaxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bcodsmox.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hptzlljr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaaedbdc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jmtlqlfa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iioanfnu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lphiqzbg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcvaozcq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3juofpwgp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3thfszbqu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cjnvrvxh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gdcbgstv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xhpwdubi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ejvpvhsk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dabzqfvg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3efynwipc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfutnaak.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vctaxvcv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jpgviqhw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qqokpeaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rqghxuxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eexngwex.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pcmxooja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cccwllro.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ptmeoarh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3aeozpofe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mltsdyuk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ctlvksxg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3liufqovu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikhstash.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rxvekpzp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bezbxzja.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xjiqlgug.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pgbduslk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bmndgczo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ctpvlxvx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tmupcelp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3degorjkr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxsazahf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ytdidbmn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dqcbqzsj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zhjwkbyq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xkaeanzh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xhuepinh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sjqftqjk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pnmeegbp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bgdszgal.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fnfnxxoe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jsvjdxkg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ffhwwicd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nbgsopcd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqrxzivs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oeprjokb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mkdtwtbl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vyeetqle.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqbrdb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xgvmotpo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3liooqoew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mzftvfea.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cankfcry.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yisjtnaa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dsiyktfi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3paipbofd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3khtnemoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3slsilhay.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xcgehsze.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hpsfdhxk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jzzjdter.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhdzxpof.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3plyfabbv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tqewqdaw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uapneyyn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nboxqiec.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3monxhjzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ntzbluqq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3knjqessm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqxzidmk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3prujarut.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3azfyhlvq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3prmwthrz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3clbygrcx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pcrlgvvw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hfifoqno.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3miiwuwqt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qthzimda.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxdcsjuq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3otzgxaeb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lzeivpge.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bikvlisi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qetnhtnn.html


<!-- 参考信息 -->