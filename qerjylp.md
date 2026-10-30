代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gmtzfflfk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gwsyfuagz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glhnpssbd.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gpxnxlfwi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gvrtsljye.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gnjmepptu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gyvuxurag.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gccuqehpk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/giwrktyoo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gxcerpllr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gddaomctw.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gfxjwfytu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gslmbcbwy.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gphoroqfm.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gyithkfwr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gokzqsoco.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gpumppfej.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/goegknkza.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gfjwrwsvt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gknvhlllp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gkwsavmfn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwkssdxbi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gdchdvrzd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/guluphoum.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjtxsyg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gqubrhwrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gtvyycyfq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gfvyduypy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqufmdu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gpguxpwst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gvnjfoyqy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/glaqndlfc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpfmjeqi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gkqgqyhcc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmjgiramy.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gyhjlihhd.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjpdhgwsx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grgdtjscv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gdvlxgorf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gyyeldxnf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gnpcryurw.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gsyvcqyja.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/geolfmywn.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/guxtuwhkq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gzuqtqoob.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gtmjnhchi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gwbsxmgxd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gyvotrsod.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gxuotslch.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/golwwntbp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gmdssuhwu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtmyqbjvh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gbwxrafwb.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/genqdielc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gdjhhibeh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfyigskjc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdjylpqc.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gxywkqfrb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gbgtecemw.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gdhcbcrdy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpewqsxll.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gwlntruwp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghtfnbkkd.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gjedlxfub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfgrbjbtf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gpbcigfxw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gauaqoglp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gvwbhbova.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gekimhccb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/ggnopdrth.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gzlsqxxhb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gssuaogln.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gkkyjzuaf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gvzhpvamg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gzignozen.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gjztbwgmm.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaftikdzg.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gebvkxlqu.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gykbrgdhr.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gmbtgplqa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gdhobikxj.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gujlanyks.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gfaghrcmg.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gaytajxov.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gijtfubxn.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gaekrtgoc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gdffeekdo.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gpqfkcnny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gurphrkow.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gpqkfjvsh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gmdscbgrf.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gfheoxtyl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gijkiwjpg.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzwkbbzei.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gztxpvbjd.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/giqayoxwz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gphuplhcw.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gvznubygt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggeegjozu.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/grokmttsa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkwxjnmra.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gegcsgozl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxorsmajr.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gukzxbpxh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyrqbjeyr.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gucqhviyc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwazecieq.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gaqsoealu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gpodqmojk.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gtwwhkcnn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gykyfgkgn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gdoptnkty.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gcysscmrk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gbyqftizs.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gynnrxdlt.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gvnliagip.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gysplxpmj.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gaxblwqcz.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gqyqamcwp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gstsxgfgs.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/geujyeowk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gtjfhgolm.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gjpjyjtpj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gqriqilpk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gnvkrrvel.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gjbviqfsz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcpexbepm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gogxqdrsz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gipppscum.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/giycjonvg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gmzvvzwcc.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gvzeuothh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/geodjxdoa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/glkkeuovf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/glawglkxi.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gbhjaosum.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gibxshyav.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/guqixtvxu.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/ghxgsaegl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gclarjcke.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvqeiadti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gipagjhfd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gaxlnqqth.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grvpbydzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gmrvbzvhi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gvpaitqxq.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gyuyczqlw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gxmzshmsz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gtvklglgs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gvrfaxttq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gifjhpdqe.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gkjhxjsfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ggtmrkgyh.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/glalronsp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gsnfbbork.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gwyfedymm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gqzucfats.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gqxrkupuh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gvhrggkiz.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/galbwikjo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gddhzdfnk.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gxnpsjxaq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gpqfkpxqo.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gwjxjzgli.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjelrfw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gnurfyxym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtvcojukh.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ggggqatjo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcrdceokn.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gdiirdpem.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/griurbquh.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gegjsqgdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxvkwhqwh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gwqjqzrzi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gjlnhcvhe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwdknnrdi.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/ggtaxeqlk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gaguhpbgg.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gsyvnufic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gfyckenfp.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gykwcqeuw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/grtkeriyp.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gqvfqdxrh.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gvqdrbhkq.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gznqspimd.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gfwfcpmbv.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gjdwoqklw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gzdmukhnc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/giibfcgmk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/guwninsks.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gohykyzel.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gpwndufcr.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/ggiysidnf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gibsugngg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gyucithgk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gfqicrofl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gjxgwxvgi.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gzyapllja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gmlwjuthc.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gpxfeavkz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmvwshohd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/ggieilqrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/geukhbxdb.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmyhdwphe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gageczlry.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gxxxkkzth.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gugfjqsuf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/ggsznemra.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxaoxuchm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gixmmvwmm.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gclzwicoe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gevcqnvmi.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gsztgxidx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/grwdqoyhp.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gkbjfkmih.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gbuwstfiz.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gslysbfph.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzudeorqk.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gpfjqkysd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gpozvczjw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/golwsjymz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqlfpvttj.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gmnkppvgz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grcseopbt.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gugkwibgi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gngrqqroh.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/geakhetgu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ghsyyjmul.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/giitmfbju.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gowwflzdo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkzqvqkyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/givqkrnfi.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/grjbuhtit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gnnyajaje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcdvadhwd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/glbfzxxjy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gjvdpxdtz.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gbljwavur.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gnnfgjqzg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdydzfxiz.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gjhgwedaj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gisxcdtps.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/geykhfgjk.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gpuynwjrw.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/glzhicexz.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gujwknipn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gavhqlvfo.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gwdjkbnlk.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gicuyqyur.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ggizesowa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gtjxbvrks.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gylwrdmjm.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gjlezzbwg.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gxhzufgsw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gxyrjunnw.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gsycbpkel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gqdyhcuwj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gnyownfgc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbwuirihc.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gaqkfpycq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gxbwalpjf.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/garddbcag.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ggwhfjosx.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gwkamktds.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gieknrszt.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gotmkncrj.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbhjayhhd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggbeyfvrm.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/goiuzcews.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gjubkjwqn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gbszwtfkg.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gvsjxxdab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ghlixayww.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/ggpqrwbje.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfddtozch.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfgcczwsp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggactokoq.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gamnenllq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gsglbnvua.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gxwtsrirq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gugwhbera.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gkxfrtnnc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gfuisiqac.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gehsqqzqd.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gnypvwabj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/goiwsvvwc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gelhpwnsl.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpugnkegi.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/glkwaugvo.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gynvxojwo.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gfxpefxch.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gyvzkwejk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gdwxyvzsn.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ggcfooapp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ghorjgvyi.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ggcdmqwfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gkuhaxboh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gjscjijsb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gfeqhgfol.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gaejmquqm.sHtML


<!-- 参考信息 -->