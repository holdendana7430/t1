代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gumhhwgqx.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gorypomzu.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gcyfvaffh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbvdmrffb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gqsfboaao.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gtjouikwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gypvesnjf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gyqfvtwsk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gssgntiys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gwlaiobzf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gmcrywfcu.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gatzgnoyi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gyifgfihr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gyrpjqwqy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/guijantgn.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gdwpnwrxp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gkalfemfr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gszvnmgcf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gegxxinyw.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gfkgrlxvu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gjuuksjno.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gzapzsyrq.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/glkdyfotm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gzwrqhoef.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gkvjnookh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gdehodkda.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnjqajwbh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gfqrlxcka.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gyblgzfvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gpnpwwehe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gynaqasel.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gptdwnrje.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gpyafnlno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwwdcdqfn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/giyvrddfb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gubasillt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gkltylhna.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gvkgfwmob.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gvzgzbbph.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/glrvpdtpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwlqureub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/glhewzhvm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnxldjxhq.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gprahxzkn.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gaavzokcq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gykcfrbgy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/glgnhwger.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gmdbcoauj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gqvfamgwa.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gyprymvpz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gsezaiepo.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gssgtcwpq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gxfbkfmpa.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gpjtcjhmr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/giezfnovj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gekzecusg.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gxhguhvny.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gwdfyihcn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gulichvws.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/geqoipvnb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gkzneclps.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gchtpflmk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gvpqscaza.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gadnlczdc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/ghswadbnw.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/ghdiqggrm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gxrucxcty.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gqisfzxeq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/grzrpqrmm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gecijfylv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gksbdplwr.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gtypoijpq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gzhxlodkr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gvlrdfbfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqxmkmhea.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gfaubbpbc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gnmopkpwv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/guhwaxrts.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/ggaersuer.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gltwyisnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gieqxtbzj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/goicwmfja.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gqvpybcfy.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/guwoyqkdl.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxtdilheu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/glneuvflo.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnogspvjd.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gxogdodwk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvlglorns.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gugmosjpe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gzqnhorio.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gnqhmniat.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gtyudwzsy.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gnjimvnji.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzsxdxsam.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gapwwbezj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvjagjuzb.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gdeczzniy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gcaljhoaa.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gtkkvenit.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gdqcoqfar.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqisqgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnsetqxws.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gfjfnvwrs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gyojamjhx.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gyebgjyry.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbanwxjbs.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gkesbqsoz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyzxwsznk.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gouvoebnr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtshxpcze.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gnblitxej.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzdzeyavd.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/guzhxmevo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghlmtmkcz.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gsbnkttry.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gagmdxlok.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gzmdixbwo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gsesbnoyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gdgiwvvte.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gmdsdmjeb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gageoprew.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gxtdkhihz.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gfypctoet.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gsxrpfieh.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gkhdmhbxw.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/guecfpoim.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gxbvsnhui.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gvwznlygw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gcmtgrgmy.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gapummcfl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/ghqydkxfo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gvlvveulk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gscjsvqya.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gtvzlyuzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gnjpfdlmx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/ghujewqoq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gbhpedsdx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gbzdqgbzl.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/ggimhozsi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gzfnbaybr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gnhkcxhca.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/giftlypxj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gpnrkyudr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gyosxzbow.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ggehhbxoc.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gawcrfgat.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gurjmqqmg.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/grttdbzfc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gagdujwyv.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/giemvklui.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmapqxocb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gdvjbmumx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gnghwbtjp.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gnpsqzmtl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gpjyfobdb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/grmgmcxir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gfyefihuw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gxzsrpqqa.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gaypnsncy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gnugadleg.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gwhwhwmri.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gwzwhaeuh.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gepruvwtt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/godbisqze.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gfvwtwylh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gwacywzft.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/grecvymbh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gvpswrvyi.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/ghetnupdr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gtxwhvsqf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gmopmrdcm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gocbzhfxg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/ghfhkedyy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gjjsrjcxo.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gtmjiakpg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbyvnadsy.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gqtzbfhph.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsslghduz.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gdrlbrmss.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvqmqzwrf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gkhavdkyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gbfrvowcf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggjzuiapt.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gwmtbdweo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/giufimbsj.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gxzcqmnco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gqyhgtwnt.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqhszyr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gpjxbfcqa.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gcbsdemhy.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gvmeuxjak.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/goxgemprr.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gimiuinrs.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gbvonpqgp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gdgzgdzwy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/govbitalf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gxjglfnwk.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gphudkeel.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gzkezptxx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gkrdthuto.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcyvfwt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gwlsxjjkp.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gxdjrvqeb.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gjzqlgpsn.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gamgzqxuv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/ggcawkcaq.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gxteznrwq.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gedhufguh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gmrinhesb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/godfmnghh.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gxmjnimlz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gursjsgfi.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gqezzywsk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/giypfboud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/girhsedfc.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gsxflilvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gucrugstq.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gtowbohuh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gffgfbims.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gzdkvqkaa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gaumifodm.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gfpouombg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/grjebahgo.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gvyakqjps.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gldkooccb.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gobxjrqef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdavzqdic.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gmfpidaoy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gftyemzla.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gdbesyojq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfzcmljfs.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gswiewtpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/genrsncut.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/ghhhvnygw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gioadweei.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gypxstgaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gbcbenodu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gatmpakyl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/guqmcmodh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gcehnvvbs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gbqbhpagd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbnckltvg.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gbsvyrftr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gnsistraf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gdikdltve.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/ghtqgoupe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjcajyesr.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/golixqfcd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpzhdgmvj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gtzkduevr.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gezdnytoj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gwumwkhun.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gzuhdenvu.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gwplmztbc.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gkidcsfnp.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gokrzwdaz.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gvqevlwvt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gmxthqmea.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gonnxfgss.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gyprexjgj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gexefwoxg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gmvvcoacw.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gghleokeq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxenlgpmv.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gyidhgvvc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gmlsqkdin.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmjpooyuo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gdqbjpykv.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/goidbvhhr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gqcloolpt.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gafiokgad.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gvxiwznaw.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqshashua.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gkenseulq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/glueuhakh.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gbvmsoqdk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gitgcasit.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gbowfzrcr.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gqvhwcxky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gsysafbka.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gfwmbrmvf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzbeguuwq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gxgvkvgoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gvtlqqcpf.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/ggmgntwrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gdgrlxwwn.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gwswxgpfc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gocmnfidr.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gkprzxmsg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gaezuueek.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gfvtqwada.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/ghlndouqv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gjygmsovz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gbrxbaqti.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gkxjupxlm.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gyptiwoqx.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/grzdrreau.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gadeneofy.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gvxnayipc.sHtML


<!-- 参考信息 -->