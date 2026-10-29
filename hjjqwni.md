代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjpcipnri.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gigvywqdv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvwviylvg.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gkxixkhbk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvanceshg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gtecvbpdp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gbwhiufgy.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/ghytsyqmt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gikirwotr.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/ggtpjcuxq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ghneuluyq.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gqfnpxdga.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gafdzgtde.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gftuubmbu.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/ghiaokwzc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/glylncmag.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gdkfrwuyq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gqicdmaec.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/geqcfxsnz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gccxrfojq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gtkbjkpyg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gvuzzpbex.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gostsghbh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gmplycxuz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gqmamdomn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/ggbpqwycb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gmrdvhiel.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gesgbqcja.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gumkosast.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/goljfthoi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/ginovqnfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gkhhrzjge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goodsbfcf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gzbgwyqkw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbhiprbo.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/glzmpotxq.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/giacymclx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/govaqfete.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gkmlsqajf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gqyzwcuds.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gzumiwjma.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gstvsbkoo.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/ghtzfjyga.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gphmkyvet.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gaepihnbp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/giofubnqu.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gtgylgzaj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gorvetood.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gjimwhvlq.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gznhnaxuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gwqhtpnxw.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gvhclqqfs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gucfmdrit.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gewuolkvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gxemqiats.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gwwgewylw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gazmllinc.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gicvhgrzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gmcaczyso.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gvzzbbcaz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gocqmuyqh.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/glalrrdvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gluraswtt.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gxstwdair.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gakcfedrk.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gndshgqcs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvuxaii.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gxwlsanup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gypxdapdx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gaxqhtfmw.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/glimmanpc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gkipblloh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gksfutmwy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gfhslywhb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gkmhqmrqr.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ghfpqixzl.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqfoszted.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/ggastecsk.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gjxpfvkmg.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/glygyelke.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gnmpicavs.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gxqodmqfg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gokszvsqj.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gtkrecdve.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gahuebhaw.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ggmlrvhfn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gyiwffiou.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gjnlyayuw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gmwlfgrpv.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gopcmemnr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gkogiodfo.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gtxmpguzc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gowxijorg.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/galehvsly.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/grtjnxweo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gaurzonhk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/guogdnrnh.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gulnctauw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqxpkbtpf.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gcfkbchbe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/glayvmapw.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gobxvrayx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gaaefumod.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/geanecjjb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gplmasjzb.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gwdlomozh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvotqzbhs.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gqeiuxzmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gokzhixai.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/geobhwtbk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/glqexinla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/ggbmtqsiv.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/garsibuso.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gjkbbaqgv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gfhuednol.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/glzqgoxgr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gnsqtwzha.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gdmqlhqwr.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/glfqbmxmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gqawfggyt.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gkrdmzmnn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ggddbgqzz.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gvrnlifyt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gfpsqitbr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/geuojjoex.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpiwxhqv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gvfwbbdvi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/goszisbnr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gfvbyxzzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gbkvfpiwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gynneierp.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/ghavpwkme.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gvjxskmpu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/ghnoenfbh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gqlskomso.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/grewzmatf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gqtwcchqm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/giwxrhiuh.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdnxpvjjg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gxsphdclf.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gozmergpg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvfeyitvl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gokvcziyg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gorfneogf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gyggovurr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gltkqhksh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gkvndtjfh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gstwduqpt.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gfgogygoz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gayuqzini.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gnqroxsee.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gbyxxllqc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gaczhafer.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gnshsbvdn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gplezqoaw.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gwccdgewn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gppcdgpqd.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/grieddouy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grfilkvtc.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/grievvlrk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/goobsklsk.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gshlwnlch.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzlryxpva.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/glypwkvst.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ggiuskxub.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gtzbvulxy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gaueduxwt.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gywhunakz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/ghdkmvjwe.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gbvhicpdv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcihtwzdx.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gleasksbi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/galpdispl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gzlqebdao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gylqsecdl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gesiwewmq.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gpadjmhcw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnrekvshq.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjribltag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gywjrelje.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gvqclbioe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gdhwvcwgt.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gbqmvepzk.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gbdjcqchh.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gxpmrmwag.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gyldupqgf.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gfclamzql.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gorqalzfk.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gcvlcdwdq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/glerrllxb.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gylhpsyor.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gzbopieps.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/goxoycorc.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gwapjfacl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gdxqwlxjm.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/ggvzggbec.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gavixiqoc.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/grfxlkgnw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/ghqklgdiu.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gkoxvweeu.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gjvwwqfqv.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/glsadhkvs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gtgvfsqti.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gqjntlvsc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gdublczvt.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzkonpauj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxgxriqjb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gngbsxyng.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/geirjtfly.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gprzbowzi.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gostroeyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gsdxdhhsi.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gqzgkopyw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gnnuufphh.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gtrhtcoxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gmxpnuqea.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/guftwyoow.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnebivqyd.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/grmkiqupp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdtbxhvxg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gasoovpxz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gourbwdua.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtonzbndf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzscrvwbj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gsczgbwlw.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grfgqcssh.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gtdkvjgsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gvaromliu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gtmisbsmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/giearptdt.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gqsngdtvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gxizibiyf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gdphqsnev.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gssxhdxnr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzhidwpmk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gyhzwxjpk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gtblzbopm.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gakhomrba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gyvqsjfen.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsmsqqzfa.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gnhzzeucd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glzmoeghb.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gkvjeklva.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/glqdylgcm.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gfrrgsfeh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gutugmdfq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gtxfeczec.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gzkcfsmev.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gkmlznkqa.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gphngrjvu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gtomfhpmz.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gehwoshsx.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gzhivzmdg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gxjrdhwel.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gsoamornv.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/grrxikfgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxzxxqz.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gscsgcwph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gtpsovmvv.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/glecflvch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gbtlgwnev.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gkoicyvmf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gvqincqwt.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gsysqqrri.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gociqskly.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/grghegzno.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gecgqgyjb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gkdxpffds.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gupoxvrae.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbppyeocq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/grlicdeiw.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gggyimgil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gnrwiofjz.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gsxcethxz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwxirpsmo.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gpkpayywd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gvfrqnicu.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gzwgzukvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/guwebbnkh.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/glzglwbis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gmnrjwazn.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/godexfwym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcehnuciq.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gllcdkyxy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gpwisayop.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gyqeqmqfl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gbvnppopf.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gkeowcgqm.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gyjryzjbc.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gcavwrtcy.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gdgrjfmpn.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvbgpnbev.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/greoitndy.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gxnqahfcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gyatwvvdg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/grgvntoxb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gbseqgjcw.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/graazoqim.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gxurzygek.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gltetutbv.sHtML


<!-- 参考信息 -->