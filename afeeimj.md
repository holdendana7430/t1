代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxlqcnjsp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gyumzxgyl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gojqfyxak.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gpojkkgtw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gpiyjmwsu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gzljzqine.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gkhcyhihf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gewonnwiq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gmliqznmo.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gmlldnres.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/geqougvwu.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gprgkvups.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gghrtlxnn.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gtrnsgvgk.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gzsozkayq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gokhgubvy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdwwace.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gwjdmueot.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guqmyzxvu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gdltmvfeb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/glizyiiif.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gdjkpfwsy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gbycqzfax.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gwqhxhhpd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gjggshqcg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/guguguanf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gfyhiamfx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gvyfqclaf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gvloczqrq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gmgjrulyl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/geysusljo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gcpzofsbn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giveuvedu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gfrysbjgv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gegqgihws.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gvxemocst.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gnhzawzsh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gkklgdufs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glaxxyauz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/grsfzjsnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gasxgksgy.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqqqcvplb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gcuashfhj.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gnytvghlh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqrttnpkm.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gayxvjisx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gqqlpvcga.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gmfoeqifz.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gcolzzqtl.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gsbivfted.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gdeolspya.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gynxqkmlz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfwwqapnt.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/glbhbhate.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gezvlqnmi.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gyluaotoi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gmwetuoyu.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gxwwmvskp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gtiwoxscl.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/geqzqxeiw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gnulvzqlx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/grejtcljc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpwkpdzmw.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gvjkumefs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtfniwmdl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gubdofvvf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggapxhtuo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gmetituex.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gqpgukftj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gjlmuixgg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gwsnktjaz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghxmmpmtl.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gkjvyoalq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gkdhrowgq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gcophohsa.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ghtwxgvzs.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsjpsmngq.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gatakaygn.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/ghykkkaof.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gtpnqikov.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gldlpvpaz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/givjplhfw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gvpdevoil.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/ghbgejlbd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gfmwlqdlp.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gzkyxqbev.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gsejvuagm.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/glpaoaxyy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/grfdicuxa.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/ghxbacbhd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gizefjvzb.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/glqmnegqo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gvhckdctl.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/grtnkjslw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghlveggzy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/glnlzvuzo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gacqvdpuh.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gcimusswp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggjdccoro.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsyfmjbjo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpxjgofwe.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gmirygcfx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfpmatpdf.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gatzusexo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkluwckua.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/geoafdodh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grpoqnzbo.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gepenbtro.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gffddlvib.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gkkchwktb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfwqosl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gyaphrhou.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gnjhlcojh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gymnjzqkv.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gdolrkojf.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gtvqnagfc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gzswyxfpd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gazljrmjh.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/goyudrfbx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/ggokqkmru.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gzxinluqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gticdkjnv.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/grhtidjad.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gbnhcsuxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/getlqsrnx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gsftohbpu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gusidrtjs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/grnffhcxr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gsuutfnsn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gxitlomsl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gfedjrhei.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gilcegnor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gnijzkplx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gnlwcxmid.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gunkweskr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gpfzetolc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gnpszltmf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gvasipwne.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/ggeqgwirr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gqsrvmrwy.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gvmuyxtah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gxzupgnea.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/geztnisrv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gyztkzcce.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gxluedtpt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gixrakidc.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gpbzigaaj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gjuwvfbgf.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gnwapxdya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/glcypdjbg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gtztazuta.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gdzybxejo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gfedtaggx.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gfhefuzpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gcqsvdrxw.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/givcbkbyv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gybzmjxwc.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gzyqxbkqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgkhznl.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gcxvoyqon.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gwiwnytpg.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gjvfqzzav.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/grevyfprc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gvohsyqqs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gmemopzvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gjomqvfdn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gvybmuisr.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/glyyyakli.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwsyonbit.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gcreshceb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmkurntsn.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/geihwzhxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/giewtkhpu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/ggtcekzna.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gxlobykdo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwoncmwva.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhtcoge.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsqvaenfq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gavskemvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxiuqrvze.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ggmxticwb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/garklnwmq.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gwctwljym.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gaoplkyzs.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gtobjawti.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gtqyzxvgs.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gcjtvucao.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqmgxmu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gnuoyocjb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/glbpvqxns.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gppwmvslj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvwmzsotf.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/geyzhfgeq.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/giuohdafx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gasozrhtj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gimyedrbb.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/grhhughwy.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gbojqxqrg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gsrmfibdx.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gnyopyeip.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhesqljl.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gvopzmkcx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gkjzyigyu.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/ggdbhfihg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gcailqadh.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/givvmxnmd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqitmukln.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqxqtwx.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gmsgsvijo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/grksmuhdh.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnxgkzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gdkpzzkrh.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gqqpsbpto.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gmhzzjnbw.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxgunuurr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gzlnvxbji.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/geqqfrqtt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxqnlnrxa.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ggborfryk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbgvwvnau.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gcpkmwgym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcahsljsi.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtsnclziz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghameiuan.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/guqnofrlm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gynoscfhp.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gxisobgqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gvywfahwe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gekaouycz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/guwkbgaim.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gixcodbdl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gvcdospbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gxcjbnpqt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gjwzakvlq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/giznennpp.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gcoyjskct.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gspdsayvh.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gsbbazeoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gcjziwcrh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbuwokvn.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gaacikhrb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzlleltql.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gicblwhew.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gmbnoalqm.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gqweoauci.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtpmxfdff.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gqvnaaraq.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gfntljvpb.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gbwlwsokl.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gdasugmfb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gbnwekglm.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gnoswecrz.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gmbcbkxwx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvqbdbgbv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwbfzbei.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gixbzmuiv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gubbcbihb.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gqovucers.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gkqydyxha.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gelvuiiua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gcjlrjlmu.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grxzccaam.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gxfgnhsbj.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gdkbuajdi.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gwwnqfqnc.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/ggeywqgys.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/ggqipvmoy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gcdropbce.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gkeghmedv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gtlsxkgxk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gfpjenboc.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gvgykovyj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gmchmihgt.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gaydecrpq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghfunpzbk.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ghownbmru.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/ggtquxisd.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gpcxnsjmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gusdhpwrm.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gapqcncuh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gsgfpnhbw.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gxthmhrdd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/grcvrzcwm.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/geekaxupu.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gvpugubrn.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gzgoskulw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gxntfgvyz.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gubfnvzim.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gdnuovshh.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gksfgsvns.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gczqrfwoy.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gibtmzdkj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gvvyevfoi.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghggkpvyf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gyqgamwkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/glkiwwqkw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gtrjuvljl.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gyujhgzzj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gbvqgdxup.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gcrhtdwho.sHtML


<!-- 参考信息 -->