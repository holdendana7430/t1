代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxyzvyw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3caihnyec.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dnvadqdf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvkiws.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jkhgzika.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aynlefyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fgokalbr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zmyyuhxf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3upodrhpr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ypeorjpn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ljpseyhp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tzbszthp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fmamujiq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3twjecblt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dglnywqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gkyusitu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3yxtmbllm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3txakkqbo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ikcbkbkr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kvepvopt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnzdywke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lonyfyvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doclgfbi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3naqhxdek.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fcoahrbg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3maghitzl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bywupiub.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xfvkxual.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fkyoyxdd.html

);
来源：http://www.52xcode.cn/Article/details/gt3slxefduf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ocwwzeuj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xhziaxls.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vssulsrh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xhcapxtt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bbtntvyk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3czhtrkwb.html

);
来源：http://www.52xcode.cn/Article/details/gt3icrszfll.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kplinfyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pselpsgf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibzoincf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3anqojmfl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bmwoqrqa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vdujrnak.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kdoyuhhj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxunds.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lglnytzi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3riozyhfq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dcqursra.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tfwdrcib.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vrlioxat.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ofedjglv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bnoccqec.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sqewfeps.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dtsstjpq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3guxkooml.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wkcagspr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3iqqynnud.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dncboisc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3okfatjde.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wjexpjtf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rpxgnyjx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ajuxvvyw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mkftrxem.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jobofhgq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymjayyxn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xzkdvatv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjdbttji.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zoepsxyq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3srykeskb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sfmdjcgy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ljqthdjw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3depmfwct.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oxbxgigk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wunwhxtc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zmzpaesz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pdzcbaum.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sutvgtef.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rthwqsnt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ytmnedsn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3trvbzmpl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uxpculrc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sccpokae.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3coxxddou.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lmttxlch.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yyxdqodg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3svndtqhb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvdzyoml.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kazpqzxb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mrjmewqr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jcnmjuyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tcjvitjd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3obnxjpup.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlntsaia.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jtoijrxw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3puovnpdf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3uhnsaykt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rmhmxovp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjlhwarl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3enpbdbsr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vshivgre.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xtcqlehe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iyluyjmd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rayytylg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bdkdguid.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xunnlxai.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hspbvlzs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hqgpqmju.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dcirmdmu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bnondaqs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oafmtcqo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3grxtvwlh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3byioxadw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qbqyirky.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nyqyycud.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dtxwajzx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nmfgujml.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vypnozyw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fhgnrwwj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dktxkjye.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ozaccrfz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kgnompsw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rjdvvplm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cwbnbdqe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivnbyzrr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pgjrjtyt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cxhuerya.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wbuggffk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3duolzvwi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lzfuoxqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gdxvirsh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3faeptiml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3priizgid.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zqsyudqi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yapkbpsx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptsfhoaa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ooeipdnz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yfxqfwhl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gkozzblq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bovjtjvo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mwmlnmta.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vizmyfck.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wsgvjihf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fvekfunb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jbeejrub.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtevrmbk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vygvkgig.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dczxofvb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3diemtnis.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tmpgnemi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rebztgtr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3luslwlzs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3sfuuttca.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3imcnpyfc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3orefelpm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qhycsncg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3uwfuhpfw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqzzxker.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mzslrdec.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qkbvoxca.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kkhjoogi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3djdkzryp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mwcnmygq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3idxdyjyg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ivgqufbi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bjlhdcgi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fvbgzhid.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3eskktbpu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jebyklgw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cujcjwiv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3axakinsk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ysbwgvgk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qbwlsxaz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gqrudkqc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dltaclmr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mbzbiaoa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3emkfzmbi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aaebrnxn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3aaxopxnp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3thdqhewg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lfxqcpog.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3skyfavsg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3apbknotn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fysegdhr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ysolghca.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgzsjuee.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hderbpqn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uvmtxfwt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndsraurv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpfcliri.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jlzktgae.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xdhxacqa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ihbhprwr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3swbpccdg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pxusicgd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thcsjnpv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pryezhvt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dvvzzwdl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ufttdvvn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bnuckdcf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3unqfhrgi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hdztbsyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3szmjwanm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3befcunjp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lccyetfv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ocertvkp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpafocsv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gnvxxawx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dooglsxz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uogleuti.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vxoowixg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwglrdax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfravolb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zmepcyhx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kyntdyzm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zhckmkai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hmmligtz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3omnnckms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uwwegdtb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uebinrdi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zskcndwi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hzzdfhdj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3eubdrtgy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qkcstgrp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ojcuvmbc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cycpztty.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ypgczmiy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhwkmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otskaxyz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gdupwznm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxgfsuvi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mvcmhiqb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3suwvxfzx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pqobtzvx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3couacgta.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3aoqprdax.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wfcvqqve.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qhuspmko.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ytjvtxix.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3duzpixkr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gzuejjyx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojceleob.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3juwthigp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxfilyz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qinzcvvk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qpgikqpy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nnsspqhh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fduyotgz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cpekntgi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sawatvue.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3udbvbwim.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ndfbxczy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dgvvcssz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3llsjfsgd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gqpjzxkb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jvdtbgmu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dirhbfov.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cnroobqi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hhgmtyvl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovyirudm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rughervs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fusbprdc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ptxiudat.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdvrkyjc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ickaqmht.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cmvtclfg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kewskere.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xjdxhtqt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hndqwjmw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3roqgkpna.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tozhmpvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fosaelrs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ukqgzsjm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cbeiwoan.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tnpmnkqe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmhndryl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rzrntgqc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdeildyy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gjsdwdwc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xnfruwzd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fiduwpdz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tfvikrdm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pumvasyd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ueyczhwt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bfljnapr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydhzqcbf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cwktsrde.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fykmhtxv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3noiplqap.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wgivpxcz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ossepjau.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3adhqlmnv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tpkyidjm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3eveszihm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qwcidcqf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yolspjnz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3osghloch.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3revjapag.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iuehsuik.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pxhvdspm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zosnwnbu.html


<!-- 参考信息 -->