代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/ggjmdqxev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gyjsibdrg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gudilmnns.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gdrvxqojb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/ggdluednm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gacwtjbpe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gislylfxt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gbvvuousd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gzneusadr.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gvwbmtkmu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ghkleczzz.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gdwcwevfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gdriwtpye.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gebcmikbo.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcghjysci.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gkbuwbgpo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gqvrbvrwr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gnfbaaspg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gfqzmvprf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gwesyuhiq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gdtpxyiaa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/ggtdkmyrm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gsbbivlbm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gvmvjigxi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gpznyvmuh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gfpblmgny.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gbccdsmzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrnayntz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gcgcmidcr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gcfmjride.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gevtjjdaf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gxxcuclba.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmrqxnqxi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gssdbvvmi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/givaexqhj.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gdkodqotg.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/govawylnj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ggoycclow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gjdrekrwk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gvjxnguqx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gtqwsijiw.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gcdmzdfbt.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gfcyiafhi.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gpywxkknd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gazlfrxyt.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gdbzzxwsa.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gaxipshwa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gecowzjvi.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gimadfqww.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gbldmxvwn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/grxhzyaor.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gbmeuijeg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gijmeelqs.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/ghjdrlsfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/grrfrzhem.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grpbanooy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gnpxgrfcf.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gxjntmrzu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gfgdszqzz.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gvxtvsfex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwhegwszf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gqvzgcidh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gsswcyqxp.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/ggjyfvqqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gbdhfesgs.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gvtnwfrwj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gliznjuav.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gdovxvevf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gkfbzyeis.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gxmryrszk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gydfjzljz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gxbyzljrn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gjubwridy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gkuecccaw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/giobuhxgb.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/grnirzsru.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gznqmpqix.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gufywvuqb.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdgbtqymm.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gkgivxxwg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gaxkmdunl.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gonjkldwz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gkiwjrprt.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gxuqnvxur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gqcvmovlh.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gsgnzfqbe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gzexpyjki.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/ghrokpwam.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/guwuuqaii.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqhopxufj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gdhpvpykx.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gogzttmef.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gfcgtbpkd.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gzsjurwlj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gfucqxhor.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/guopqyykl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gbdfyorjk.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/ggtafdutg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqvldmykn.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gnrybrblm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/grwzhncnd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gujazqwdx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkorswuzk.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gxxnpayzt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwhuietxa.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/goiqtftxt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzpprklc.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gpynwckqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/glqtnxriy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gsjtnqgeg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/grllibocz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gukxhnoei.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gbpkhabth.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gmxwiftmf.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gxhwegxpr.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gxhuxnknz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gwgjpfkpf.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gjouaguwo.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gyktjtcpg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gxhfomzqy.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gueshycus.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/goyffuqoe.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gaxxzqsli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gecfzzhqu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gtbthgerq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gdlxfgxil.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gmjifesfn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gqlldnwua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gqujmotky.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ghpcklgvn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/ghyxfxtyr.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxetkzhjn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gnepjctey.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gtxnfdnaw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gaxipnjvc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gdnqmultf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gmyhvkovu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpikikyon.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gfvohnjrk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gxuaupsxc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/glyxailpv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gfasezzmx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gzehcwhsg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gegbycgyt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gndpoknpc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gzcilgbri.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gqjvnphow.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ggbpdcucp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gyoidlljl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gmndqbmtj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gfjbkmtxb.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gepgjqzny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/grefraswq.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gewuycpix.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gjbnyfdsu.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/grkjyeifo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtwnyvgxf.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/grjovhlnr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvbyiyfba.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gbnchgcqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gmujejfic.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gihwqoznr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gmgwrqetg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gacjtvokc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/glstkpwlq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gfyirhaem.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gwploklit.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gwvjjzggw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsabhkmry.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gxnzqzmnp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gydoiyjuh.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/ggnkxwdrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/garaejlab.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gracpfyyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gmiknzrps.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnbufacmr.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/guysitysy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glikbgntb.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gighmnehc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxvrcgazn.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gdksevlqw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gilweseyf.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gofavxvti.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gkirpiixa.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gxjdxeaso.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gmghhezte.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gitfcytgn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gfclmprfa.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/ghkfcnlsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gurstdhda.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gjzfltybr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gsqwgliek.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gkhurfrhp.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gdhmnhiqj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/ggkpzegjn.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gqdgasnrg.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvleszkci.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gstojkkka.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gqvyavbsy.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gsaxqywev.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/goqxnakfj.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gejnpsrec.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gdmiftybb.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gcosjzsgc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gwtrmvdit.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gstaluqff.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyckpfgpz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gskqkqqxw.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/grxbtlubg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gzgiwjqgj.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gqisooatq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gxuhwejky.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gomtuemnb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfsbpfk.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gkuvejwza.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gfctuirxb.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gfovzpegf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnczfzquw.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gyxpggkxi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggtfybjiq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gmrsomcdh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdbiyabsi.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gvzeowcfh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaedjnxdd.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gycivivna.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gchudneca.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gauphdswp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gyunzqkgz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gciahxddv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/ggnephesb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gjthkontc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gnyddpumx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gnglzezbi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gmnastnky.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gikawzgan.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gzmadpndb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gqmmywfzw.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gzieokulc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gxborklof.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaxzarnen.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gsloufxzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grfzvgvku.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gclawhoud.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gbhxslrki.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gpsfpihbx.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gyxpcjuoa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gjftvpqzc.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gabtoxgww.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gqoczupnz.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gpdrhgvfn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gntedwffj.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gvvbsqkuk.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gbrcborzg.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/ghgwzetsg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gniwpoyru.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gnfwgvxoc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gpbmaohze.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/ggohpzmdq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gecwjpfaq.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gocpdzgeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gggtrjlys.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/guurmjqwm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggpcmgxyq.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/guingrkyi.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/goqjkogew.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gtoxhnkhd.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gwxuzvsud.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grvucptuu.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gwxnyxvxg.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gagdwtidz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gffvseqay.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gvlnyhrte.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gknkoboya.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/guenqdkyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gbudbclep.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpdupcwxs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gtegmpbnx.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gfbusijtk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gjyfrxzbx.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gelyhfdte.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gjdzywcwa.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gqaeqxptj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gsueqbmuw.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gtshwgjda.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gslimnktx.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gxcirwbnv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gnldcjglm.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gckgpzduj.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gieocangg.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gasvjwyax.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gyuzpzoek.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gxcfnwfnn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gpccjwqyu.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkzvqnzie.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gmaogxltj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gnwjhttuk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gbhbpnlli.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gmjemishl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gyswqniqk.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gbnxgrefk.sHtML


<!-- 参考信息 -->