代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2koufpdvf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tzmxgcyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jntkuyjb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2decvmlmw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nvjrshky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wdtrzdlc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xwhdggnu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcxkpeta.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rwrfzkwx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqjioxjd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qhmmccvn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocwcaetu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jgijdqef.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ujoeipsw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kqpjuuud.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2chlnemvl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2veltrwnz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lteskxof.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rrkvrrzs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iidmjwmz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2klilmwqi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zfiprfyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hpdtcqkv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2sqnoinfp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2efpolrww.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kenupisr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cfsdsnzz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbmhcfm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lbjtbokd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tjtyrahh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hlxpzhql.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jcwmgycv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqdnwbjw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yvtnlauy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqppckfn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2abesizvr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdrwjv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2opbbefwv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ghfyzacj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uwyxpcff.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2etaabjdn.html

);
来源：http://www.52xcode.cn/Article/details/gt2fpmascgt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qvxmwsde.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2txejwviy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ncxvlere.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mqflssze.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wrzefpmx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xcigpqho.html

);
来源：http://www.52xcode.cn/Article/details/gt2xdqcfvei.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2idfigaze.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ctvikevo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2gqavcruc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qtsuvcpr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zsgbeicf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tjpeaeiq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nvvrwura.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iqiwerur.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hkvimeij.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2geosmwvj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2iwbkrmjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ytrjucld.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2txczilcc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lhtwcexz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2otnlhacz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hsjskllg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fwldsyej.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iulhfnct.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mzgxsxbz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yjxvnrsw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oeorjzsk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2urkbvsfj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dhksehru.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gyrrmzkp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2humlixwp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ewlvgvty.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2webhtrwa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2utfgbjuw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ncudbonl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blcfzpvb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2erjxsgkq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lzybnpfd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2cxxjaomk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dsvwktbx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bqjfazce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cbzhmpnu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2thmhnuge.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wcvjymue.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lskyqxal.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hzpwughz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnsxmcrm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lhkzokyg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xsdptfms.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jvjqaefl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xdpzrvhb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjadrdmm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dvppvmvg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ibzdmykf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmrlup.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xkrmhbtp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zohmgsxw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfbxlwvu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mhavokxq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xvzgjoai.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lsrtmhle.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bbszgwop.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xniejggo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fyzwgrgm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2thnukfbv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2madanmiq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dwpgdooq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kmsxmuzr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2owcvfsxw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ulmbmrxk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ilcuglhj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2huhrtrdu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bfkvwjau.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2sfwjlmaj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2geqtcvgz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2guccqirg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jndxwopy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ocyibxql.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wergapzl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xcqrlzxq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wviggwlv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2czzgdjgp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uraiwmrz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hytxkdyn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eqrjkzlx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2akxdcarg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aamhjyqp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yrhspcfi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kvypfacw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cgevllor.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2spvwpwkm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bwcvecfy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fghqbzqm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zotbzilb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dthwlhwj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ovdikqgx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yszdvhff.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nqfozskv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjjuamv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lomqunaa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2viezsdwn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hhvzwnqk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jswviube.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jmwpxroe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2adqbgbxx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2giqkzlsv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2eewhhlfg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xroiljqh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2utlauaeo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2awogwiiq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sidxznuf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hbkqgjlf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2osratsai.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptuccsii.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iubvuhxy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sqjlgpst.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zafrijzx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2myrlnuju.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jmvuecsl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ponpcjus.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rwbpwcla.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sgfftjzk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fsowvdqy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pcnpajcm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lrytzlbj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psbajwru.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zqjqnxfw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntqwqpcc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pxozlesm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fzfkscnj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ofiylbgt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ebvypvpo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2brvtdawy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bfywbewm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mrtxmnxy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ghjztaom.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rzwfrevk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yyqcfzoi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vykxzdfe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qeieqyux.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kwisonma.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ikzgdrli.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qzedfetu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mgkkqbxv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qtlaqxev.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hkjytkvu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fbttjjvu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zrtgqipv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2iymfbtvw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gkurbdmo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2usdupowk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ahsikyow.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ojoyktfl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksxotnsi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2coxcuhcd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nhqneviv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wlzajhbq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iyxtxqyq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ybruomzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ipwbztir.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2eimoiigj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wrlwdbdo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uzvhsnms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2trvlamyl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mrxxnuvr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ffjtbqfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvtckj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hhhcjqub.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2npktrujl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ghhnocwm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2auxktqgf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eekhktlm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2uvfufxou.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wczsifcm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbfqexgz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gnsnvxgy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crltfbpb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qcgdffjg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cddzmftu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mvakdjvk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwpemyll.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2idbqqtku.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtyqxpdi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tohchjho.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2klgbgjbs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rwvglrmu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2avkyxxuv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2epanetpq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2heflzyjm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pyhzwdmg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wkcjzaos.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnmpojeu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qxnjador.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ibdmghib.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yejgmpwr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nrzpmfpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onxxwvyv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rrmtwcsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dquopsqr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wwluufvp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yghjsypw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hbbgihyj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2waefrbnf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gganvkgd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxoykdaq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cclvggyy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sovbsuul.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gnrfvzmi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wleqdnwc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2waeqsdxw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ffaodyep.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bqubdzhm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xdwcbmsm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fndixgcc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2psmaovlo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2uhxmfuty.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jgqdbdlp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2idwacyif.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ghnwhruo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gkguatzy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yanfkybu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ibporhai.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ephgytzy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2liuhhjcz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yysbilwg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gbvnaeef.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbbmldao.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oaarfger.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ibiqfqnc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bakiylvo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mkiuomej.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oacnrjdn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hlnaoupj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zpxbltgs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bpzbjnix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqbdfslo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vnmznveb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2royhtpce.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ulobovhq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ziavnqqu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aatfwprx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jcsgzxih.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2divpfscz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vssuuswu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2czlgebor.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jeigynjv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zhphqugl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2szomhooc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xylmeyll.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tuitqywz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fxvknqeu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ayxctdwy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2amsfuoxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvzkxxqg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2iesyqagw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hwoorbzf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kftmggcr.html


<!-- 参考信息 -->