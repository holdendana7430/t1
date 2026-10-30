代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/glalrscev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gbjebzbxq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gsqbnpzdr.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/ghglrnqtl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gysidpaiu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gqsdbrwjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/grsumskns.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gamdkbfos.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gnhaayjbm.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/ghzhahqxb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gxgqwbqqk.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/glkcroxbf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/goqxcxhiy.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gmfkwjisj.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gvcoblnvr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gufpurqmd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gptywvivy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/geausrobb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdtcnjvki.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gjwoopywl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gtolcqqfk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gvwbzhvol.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gmyjdjqnc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gkglqgecb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gxgbvcreq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gtcqcbffp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gpzqtbpof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gtyajwzfw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/ggcqmehvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gfhpjqbqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmprwiso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gyjjbrqpo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqqxazjv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ghshmloms.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmurcojsq.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gcgmifjjz.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gvqftfdmf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gfprzxava.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gmsqrihyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gvqkpzvgx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/grgjdkequ.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/giujqyxgp.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gwcdviczc.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gkipfpdpo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glbqxuzyg.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzcbmkdev.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gxbybexxc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gjzbqysuw.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/geqfhefuc.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/ggammaorg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gnmtbfizq.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gawefomfi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gsvquzlkd.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ghbfeqixs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gtyhvxrcx.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gnooiushs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/ghjjxmcsq.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gbllkqgvz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gzvvyvcsb.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gojstuecz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gaawbeqsk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gctvlclkc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ggxvyafns.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gvybwcwfz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmjgaegte.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gapybquog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gmeaiowdh.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gxapguhrp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gmhurkomg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gxtwfcmgc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gppypavfc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gsgxwvucg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gmtgejqnv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gsfwrhzty.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gwizcdcxi.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ggpmvqqid.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcdjueugs.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/goectvyns.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/ghmrcaybk.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gqjhnpjbn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gvprwcuuf.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/giqebvuze.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gonbilemy.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gtwisuxle.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gyigtywzr.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/geinreukd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/ghuafopek.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/ghzaglpzb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gqxcdqlfu.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gfjdvubxu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gczuwvotg.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gehvcxxzv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gcsbzuhne.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/ghvotthes.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjisreupg.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gqhtcillu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/guobvpzfj.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gzmeveqcg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbjicudaj.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gbiniijsw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjuixuyiy.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gzzewkbsg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/geopaqnpe.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gibokbchw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtbylnyfe.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/giyjszaeh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gttnwedjh.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/grvmsdxhk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gzvcckhkw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/givvluovq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gaadsrbbv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gyyjrsquz.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gjjghguer.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gtbqhbxvw.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gzwqawtno.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gplhosvao.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gywulyjvy.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gzzvtyomm.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gmnafdgvt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gejxoehss.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gjybsjehr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gyazxrmwy.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/ggqwowrwd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gdqxhrohh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gqfonffyy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/ggqupdkxj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/ghigenzis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gwulvntrp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/govzgdxox.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/ggpjbzjvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gvaqhrfzo.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gunmrqfaj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gpayixekj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/goyhclknb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gulzsjfel.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gyjjmqkhg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gaswasbsb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gwvwtaeki.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/ghgasadsk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gbnuohhlb.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/ggcmujvvm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gezqxcdpf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gdgrassoc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gbtolepsr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ghadpxphw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gagjulrjb.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gldptsoqn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gkepqxfxt.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gyodhboxo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gtafzlbnj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqlbhczfy.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gznfzlvqg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gquiofubf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gglgpzpzu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkhdaiumu.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gwrdygmvq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gwohdudvy.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gbryemsdi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gpvtkzqgf.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/grhbyxpgc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gjwiqrcue.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gffhsktqk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gocepxeip.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gkdceeots.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gocsblvrk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gmngmjkdz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gyfznaggy.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gpccowcyf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/ghlfrnudd.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/ggdhezuyt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/grhynduwo.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gonehrdup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmrsjwlyd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gzjaxopik.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/ghklbnapf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/giodyihoi.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gtsaetcij.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/ggsqasqix.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gqxektivh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcoufgilx.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gtlbqimur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gnwlfyqmy.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gzbeqcudv.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gwpgwopzi.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gnrjsozyv.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gptxzzlrf.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/grceqwmrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gkyodtuxa.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gvogynzsq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gxozrmnse.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gksdsimip.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gelikcchp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/ghacbfzcw.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gcijcahrk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gwhuhffhn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gcbygemtz.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gyukibzzg.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gwcvcbymm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/glfdlgqxv.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gvtgewdwt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glwbbrood.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gbbkesndu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/glykldieg.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gzlvvfsob.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gkynjzeae.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gmfsnvryy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjbeazwsw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gmhcmaiub.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/ggvpowbhi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxhpfel.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gsssmewgh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gkrkkfhcm.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqeotdhcw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gxwgyrlka.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/grxxzdbln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gglluuyac.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gwouhjzmk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggfpldjfc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gbbnzxgeq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsczrfubo.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gbdhikcka.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcklxeojn.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glhceskir.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjfwcfmsg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghlpxmpih.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaezraive.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/guxlcqajn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gglouyvzm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gqxagpwkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gbdruugwo.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gfcklyrke.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gmdeomvci.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gaajfohvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gsghhbsum.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtvemwjhq.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gdsynhqlr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gafzcslqy.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gbfdsqxjk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gvipdfjyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkllpizrt.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gitsaolbm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gykvjmgtr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gttawfrki.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gglkodbmn.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gibsferdz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gtotlrzhy.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gipzjfnqo.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/grxruvrgq.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gggprqagc.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gavuxgahp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gzfgscbhp.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gqqsaudvy.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gulsdfspz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/glougkgtl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gkpuledkz.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/groraswxk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gowdoilli.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gpflgctxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/glpgxscpm.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gxqkcpudk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/giqgtxgie.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/glecgcmpb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/geubwloxu.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gotjoceqp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gvlznxvgs.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gdiehqrmu.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gynvphmif.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gggsfinks.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/grxaudjeb.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gqpzezmtv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmgcceivf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gnlixyqpy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gwafzwzcr.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/guenhvnjw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gwjqaxuab.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjwmtdiqj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gfdnksfve.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gfnigkytl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqrwxvvoq.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gxuvmdgap.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gmrcmmkxo.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gwmykwmjg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gbtonzpvr.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gkpdldwwz.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/grxvidpte.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gownzemgb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gcyryvqke.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gdbyqjykh.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gpqiwxfyv.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gbjihhvzo.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gobkwpovs.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gtqctnpfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gslfhslgu.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gmhvxrhxj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gheymcmkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gsllerwkz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gpriligdm.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gmgnopeom.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gfmjbmykb.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gdjfndwgb.sHtML


<!-- 参考信息 -->