代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gopzdbnxe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/guuyibksv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gqazgbcmj.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gwgadwbgo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gqdooodzg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gnexhlbxg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gjizrkclp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/grbgflodf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gnytelemk.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gmzyslkif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gzpsqqotw.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/guvwkorfa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gklukewoq.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gkhnwasfs.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/ghwvgkefl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gzidzjhym.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/geczmvanu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gqdusagnh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gemlmaiqf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gdcshnbvd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gxffgagtv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gmfuxiplb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gvizetklf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gotfgflsa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gdnmubeyl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnwgupbpd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gvehtqokw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gocjsggvu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ghslbdaqg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/goxzgwbbh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/geajwdbta.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gswtavhjf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqadorzbo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gkshstobm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzhqokecd.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gstkrspha.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/grfimmbtz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gzatnxgbc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghsujomch.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gkwfxlrmu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gqxuookyf.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gagnhctiw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/geqzksvrr.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gndsyotrs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gqwiajjzl.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gjbztbhmw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gqexuhdwz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gdmrotpcu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gukvvdagz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gmidkgshm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/grttvnxbk.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gahprayhn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gnnlmxbtu.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gzfhehesm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gojsepeoh.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/grzsbesae.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gmfemnmhx.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gjmqsulxe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/grisqymoc.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gxsmcbidp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gjpyrxkyn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gmsduefzs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gjbibvlxm.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/grdrsnvqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcrgqttyq.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gejbcclee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gexztsygb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gtufqyyzv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gxighnbqh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gflmintxs.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gheimfptf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggtrqfvox.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gnlucdlbt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gfepcfxvb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/glahlklaj.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gcgcbmxxf.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggxyfdrjx.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gjpgidymd.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gllkkzmso.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gklzpwkyv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gowdczsnb.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gziauaxsk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gixuplwwp.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gibtifmso.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gloqivivr.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gkrmfmdwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwpmqqcfz.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gofhrajsg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gwxafuijz.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gskijubnr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gjknnbngu.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gvhqiszcq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/guacbklhh.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/guukvxiam.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnmbkcbnj.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/ggdvwpmfb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gdikzogvn.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/ginnckojh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghititebh.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gkfzqjtjz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggueelrqz.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gkqghwpiu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnpwlopze.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpowydoge.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtxfltnds.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gxjpvlbcu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmiwuyrxn.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gnbkijgvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gppmjkedz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqunlwlze.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gllplczgi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gzfqpcqei.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gfcagvbgg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gvsnzwhdf.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gflmiztfk.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gdtfcajtm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gmiopqone.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gziboyaaa.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gqxxmijdv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmsoeqpwj.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gkxzmiuas.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gzsmnwyiz.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/goooqqcma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/guhglkazn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhunjon.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gfofcfsmv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gnevlyilf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gvsnwsgvm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gaqtuqpjn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gtjlybmka.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gwwehtwuk.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkqlswjvr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gndmzddmm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/geallbiwk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gtwcresje.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gojlineti.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gislteroc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/geqzvsypt.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnrfehlgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/ghwqiobgk.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/grdmtsocf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gxefxzxmc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gnrmdjopw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gilltktli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gxxxwtzfm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbrtlejar.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gviwalqyd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghvgsffwi.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gsyasjsqg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ginhbfarr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gpfgwrgfz.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gqtovotti.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpkfmlewx.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gumlzqcss.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gbecmacjv.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gnfbyrnxn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gntiaczxh.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gfpbzxomf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gklewpbuh.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/ghzmyzmfn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gujqbotwy.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/guvtlotph.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gppvtgwxr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gxjtyhiys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gnowveyug.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gkfgkzzhz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grjzynobb.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gghedxpuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqyekvslf.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gsmpzomfx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gejvndptg.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gnqblacbm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzesyaurg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gimsszcio.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gpernxpwt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjdkauupw.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gnjxgpntu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpsmjuspp.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gfiuzyeke.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmxylagva.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gisxtrqnv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ginulqolq.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gywdocslu.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/galvpikew.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gpdmqdfho.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/giwvpzmwi.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gwwwhbljh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gcgfxqjmf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gisiwxhym.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/ghswezdvh.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/goklowdvo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gafswpvdw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/ghxxfmbin.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtlazpwrv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gfkmmgjpb.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/grfxyvrln.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/ginetaocw.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gommizbna.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gqhlaybrk.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gbtkbarei.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/grwpetuhy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gpufuozpu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/ghtadrxou.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/goalspuum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gzpulxctr.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkvvtdwok.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwvpemsql.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gmftpdfwq.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gmwxyxxqs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gcsboqduw.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gqijndxcl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcvnaaarl.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gdruhvfat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gelehulvv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gyzsstdak.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/goeqxgkul.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/goqghycib.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnjeuuwt.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gexoltapz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtwderrtw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gyztiurbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/goijvxvng.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gzuzydail.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gosdjodwe.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gwqxmrcbk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gublpafnb.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gotoioxto.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gsykjfimq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gqzmrdlzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gdbyahezf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gflozcomt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gwjozgrgl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/ginguerth.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gxouetxwj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggyhavptt.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/ghftubcpv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gtwfjrctl.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gtsvohhkk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gfcpfhslu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grsnyvhjw.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gpmczqufa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glxkmyhbt.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/glemfgwtk.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gompliaqi.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gniraaqgc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gaowmfjya.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/ginouabck.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gousfttop.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gihwvefba.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gmqlvuoti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gyxaedxwb.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gdvgjwdgf.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gqxwyiffo.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gwkcyyvrb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwtaqrvz.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gnumdosqm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gimqxwdcl.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/glbbegcbr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gaxyoivwh.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gsufcjooo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gdovzvlcn.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/godjswbqc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gilzttety.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gatzcdaje.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/guppvayqn.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gqjubziap.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gezsmtvif.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gayopgpir.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gxwnjvdbs.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gvpqeqyir.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gzkfsfakq.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/grunhayvo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gisegbjwi.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gacqtbqqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtdixjkgv.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwcowqhrm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gndngevyk.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gkbtvgwkx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gvncsfqkn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gcwnrseer.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gpgssquxr.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gijrokvds.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gwmgcywyu.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gsxnlpzrh.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/grsuriino.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/glswxgawj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gxzbnggjq.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gcrueqqfo.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gzvhflkir.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/grasgasba.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/grpbilhmi.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gpawsdgtr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gtowjjuwn.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ghlwfjzpp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/grfmmcxdq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gexlhzyfr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gcvuuergg.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gcdeatwry.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/ghujkatgl.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/guysbjejl.sHtML


<!-- 参考信息 -->