代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gsbpazlpd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/ghidounyi.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gtpsjpcwq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gfvwovbxt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gtwlbefez.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gpwcqnfhh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gaqgcdmdy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gjiukdwpv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/goxxeoszi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gymrawenv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ggzothniq.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gfbuauiqp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/ghyvammyk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gfaatvxhc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gulhwsqnk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gsvswmrcv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/grlqdhxqg.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gdxjtdygi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gqosrynph.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gnepuiqhw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/ggnkefiow.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gzplmwlno.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcgvclcna.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gujlyrapp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gkkkvbhlp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gsszzitmv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gurmtjgey.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsbgzltjc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gugnikdko.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gshqnyncx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/grxfkjdwc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gnejsqsuf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gamzuywfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gfzrwihdl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gofsmrhej.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gjqtoozri.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gsyofkzqy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ghujxlgro.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/ggwrofdmu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gysfrtmoq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtwudnmgm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gdkbrmalu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gronuitdu.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/grmnjrfdm.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/ghmrwsnzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ganwxrpbn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/geoqusnyv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gpowvmluz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/glaoyzlgm.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkakuvyt.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gjljaxsvs.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gbuujkxqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gautztifx.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glvlkzyyt.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gzkjwhmuz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gvfjjpuqn.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzddgwzqx.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gntwogxcf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gxdiuqekv.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghrcwefdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gursbhdmw.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gqzmijjan.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/giktzbpay.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gazsjjyqn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gfrctxtum.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/getmvkdoc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gohasidkb.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/guxgkmrbs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grtlxgewz.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gwqdyjpjp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gonlkkyzb.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/ggsttlqwm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gcpxwkipe.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gyrebgnqz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gqbpcaxgk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gmunbogfs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gxpgaskrb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gqehlrrbq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gwbtkdshr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghytwcmnf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gnoefqyje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gfwbbsksm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gsxdyyfvc.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/golbvjftm.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwpwrjjkb.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gknetnjnn.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gpakvefio.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gmewhqyhs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gzwynlmom.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gsugqzjaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/geqebhxom.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gskgvruvr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gpbthonjk.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gcczvmvrs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxirpsnrt.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gjdmarryv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/govenyahw.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gehtjrrqf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gkagykrgu.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gjzsefkys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gspzmdeiq.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gojimtnyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/grmtlvhcd.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/ggauayxeg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gwjvfzvfc.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gqdlkaowt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gijiuphky.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gpxketkni.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/garkxwmjw.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gcdyhpqfy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsxbuxkhr.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ggnvrcrkf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gictprhby.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gtyvlvtwc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gaveejshq.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/giwenqhct.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gajofxfqe.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjnjolypy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ghvtqlukl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gjphiiahh.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpfsgykei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gykbejhvr.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gubpdqvhm.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/glykxpkuu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/goxcvfacb.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gbhgxsyvu.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gmffhnjcu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gsrwdcdro.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gkczjxxka.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gryubuhnu.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/giyphqyjz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gxmfubsum.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gjfjmdlrr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gfwiilkfx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gciofnwtu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gnxhpsqkr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gaaehbmkm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/grehqpjfz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gjxwxgjez.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/grnxctfjv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/glnmypocs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gwblhjjtu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/ghqhsrxpr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/glnjqellc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gbrqapouy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gfeqhhiaf.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gilrrcddz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gejzzwfly.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gvwbbowlr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gmhzaitdh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gctyktbtv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gnllankyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gkydkcfue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ggiqxyzdl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvzpttjfm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gaiidyqtq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gzraeovrw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gsixuhuef.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gpztrzqcl.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gtutivyiw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxiazhogo.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/grinumsfm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkdsugmdq.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/giugftqim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmmkobjsc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gddbpggcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghibfmbwi.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gkogzupvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gtbjfbphr.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gcydultdn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/giawqkxnk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gzpdwpwsy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gkqxkuddc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gzhaukezk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gelzpzbpu.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gapkfhnyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtvanzcxy.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/geatdiiod.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghlgpcbiu.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gppazwlif.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/goibdxulf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gmghwhgqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gexxbumof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqraqrjpn.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gjsmlnksj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxrvdqcby.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gmgggqskt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gbtjyfpzc.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gzbldbxxe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gdimslvxv.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gjnbzsckg.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gkbvasftc.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gfopdijjc.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gieuctwkp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfywmnqmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gnolxdqor.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gghurldee.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/grkfyvixn.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/grhwtyqij.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/ganrrzdtp.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gkksaxfym.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gugkgbetw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gmcqwmksz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gxkvcgzks.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gtisszfeh.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gvlbhgnxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gbyqvhamf.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gmcbhlamg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gucyrvzjr.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gaxfxnxbi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gbnrjehpw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gefdfqkei.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gqxjnokse.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gflsmxpzi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gsspxfiiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gjintrwxs.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gaahjtvqj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gqjmbizax.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gwbgnzred.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gzdnlfyzj.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gfqqvbeev.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gsaaxdvss.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gosolldxa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gdcuvmnhj.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gqltixvms.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gezseilgd.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/goutwqsbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggkjyaivc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxiafmvwd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfcpzeirk.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gwugrkpop.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gardzsufz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gciwfguqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glddwsopn.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gajmhaxwx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gwodfsmgc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gidesxdnw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glpywmocl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gyxyylmfh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/guoopmhsi.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gralaoezz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gicnljuts.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbnkqrxqf.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gppabxqud.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gwtnevavt.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gfshcgglk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gxbmfzsiy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbyvwivwn.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/geyvhcjjv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqoaykxxj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gdovpejgl.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gehmbikos.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gptvtlpcq.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gunhfimil.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gwpafdhgq.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gbhvcrdpm.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gtylaoglv.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gceizgtaq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gqcpltfdi.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/giqzgjnjy.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gawvekcya.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggghalbit.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gyawqaulc.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gifdpgqfv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpqfexmum.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gmcvaylxm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gazzmmawv.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gdmyprpud.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gpsoicsyt.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/glzkzydrm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gugeaucvx.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gfvsoptkr.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gkdchnyba.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gqfbgwftt.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gvmannqvv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gywzhctka.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gvfyjisrw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gazgkfdhe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/grtkirxxy.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gnvtwmgre.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxmbvgbxc.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gctnvgonp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gknphpxxp.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpocwdsre.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gqqsughpd.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/grwjuhmlf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gymxjdskh.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gnevkwhyv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/ggdkvbviq.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gnutgeqvm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/godcifugw.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ggbxeksbx.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gedhrgbzd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gyvoslyid.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpoijvkdc.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gjotahrro.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gnrovjngp.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gqzeouhqm.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/guatghwus.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gsrmhcoeb.sHtML


<!-- 参考信息 -->