代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gbqcxpfmj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gdaulvcwt.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gzgltugva.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gzmweahmn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gejwennjl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gibaelwaf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gxliuqcjd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gujrencue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gypnfiajo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gnpxpcesu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gtobzrvbz.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gstziqumj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/ggpbarppr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gtnluhfoa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gwjrqwhmm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gbyncnxfy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gyzplgkte.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gaywfggrt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gdobkkthw.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gtgaflkjb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gbasqxzrc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gafylsbqq.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gwjnrzvby.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gaqwpiquz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gtcvmqhqq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbpvfejgt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfezfjoqa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gyzzhiowj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/glpteniqi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/garnaokmi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gbzqmbczi.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gcqcgmvlk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/glgzihwwn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gbbsnakpn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gzuihvclq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/grysdxffj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gkfzvuzhd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gzipabnbi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gjbdbjjrf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gcbqnyhjl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gijuqdubw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gxuahslbt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbjiribtf.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gboohcjkn.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/ghquocnln.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/glyqwhnuy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gavvdbdmc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gcgndocnk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gjuypuagh.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gnaghrnxy.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gdodjewtg.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gqgabmzkw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gxfepzhez.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gqocctyok.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gpzjshvss.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gmzmdhmjm.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gvwlpxtph.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gzgbagkxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwzrdidxk.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gwspstvvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gwotepvbg.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ghrfuhbsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gudquibvl.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gcwpbcrzi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gicruoyau.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gemctqazz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gkjvrqhot.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gsflpexni.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gwsndphrz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gfevzzzrf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gvinbzkbf.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gvzljnlwv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/glhkpqyzj.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gvhvresew.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/glowatmql.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gtamznsce.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/genrtyjwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gcquxurqv.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gszxfwfyo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gntvilkxa.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gwcpxqrbw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gekdryegw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/girtbowfb.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gkfnqkmdn.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grayndiwr.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gtmrpgjav.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxyqnjsuh.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/ghszplisj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gssmtgboy.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gyvipgwpr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gvuotolkw.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghehjwccl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gfchjzsse.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/goffzpxsd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/guriczhyo.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gslxnqbsz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqchtwrzb.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gzmgixwbj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/grqmwbzke.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gmsfumpmp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gqywlrxml.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gjnlgbivk.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmohnrjfl.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/grdzbsyii.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gaivnkxeh.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gfnhtxqxh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gavuwjtxr.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/glyzblugr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gtnsncmaz.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gzjldzdow.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdbzgpdsb.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gugjmgwmw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmrwwzvsh.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/guwdxrlrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gafoxvtrf.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/grlwptkhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gekiebqtf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvhcurxrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gsgjkezvt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gdggdzpap.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gcdrlmchm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvgvfseqn.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gkvfxlkip.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gqnypgxyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gnjtphlli.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gxrnrsssz.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gtncvaooo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gptnjchcr.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gfmdzehjm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/grxsgsyfv.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gibcdayoq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gbnvzynbm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gzkyidebv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/guwiphtkl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gxhetcguo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ghxnkwaml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gdwqckwdb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gdyvvwkqq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gqrogavyy.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gzcgatpeh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gbugktwii.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/grcgjlono.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/ggpnhjshx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gzrgvmlvw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gknhqpdhq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gdishaegy.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvgglepcd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gsvewhhdw.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gkwsctjsn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/guexoqjix.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gfspjuqdk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glnigbspv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfwrhrbrn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gokyilrgl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcudtnnek.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gxhxhlrzv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/ggvrehexm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/ghhbojpee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbqquqxdi.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gvwimrqlq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gswkmyzgb.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gzphqvivd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghsgcjecc.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gidkywefc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqcgqvmzy.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gipreboxg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gyvyfezbd.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/grdyttszr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gujcsqmap.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gkrovckve.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gbmfbtgew.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gflvixjqv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/guwxlxcdq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gugzwbxeg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gkvfpcyvn.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gdrofjtth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guyyiumop.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gaodspftt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvxdogcbh.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gyzvkouyr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwsflpowk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gniyavyud.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/guqusqqkx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjjwdwwzj.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gqzedyowl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsafegadf.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gabsotysb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gsetlzcai.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gumnucctg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gtqdtmzrz.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gbwzggrok.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gqfxcagut.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/ghpxhahty.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/glsubanmy.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/ghxkjyjqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ggdunhwpj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gajdnqupq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gmqctvcso.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gfbbkgigc.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gwhqczraw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gcxpuvafa.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gierbhzel.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gxsfckewb.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gbtfjmbca.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzhkglakw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gjmmnpogv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ggszjuyse.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gnpovtils.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtnigwodz.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gpgdatiob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gunjraekx.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gtmmugkfv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gqtdktrco.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gmgccjhof.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxycdtnhq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gknzxbnrh.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gzudpuull.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gicxbwfzl.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gulavjqxb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gijimqwex.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gactkchgt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gtiaffrib.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gxmxjbelq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ggwiakhds.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggaiorzoy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtejsaapz.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gsrqbmpmf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gdsmofdyw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gejdpamhw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbgxmdaxa.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gvafllapt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxdawzyzc.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gyguivdvq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glijagvzo.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gsisfpyjw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/glpcagfpv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gcghymqzt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gcqeyusbz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gqpydcaud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gygfbpjwt.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/glfeexaqt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gxnolhhtg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gltctdrdt.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gavwoezxp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gcsdrvgcq.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gssfkonvg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gpbqgkvbk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ginxawxbv.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/geyfmfdzj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcclqcuxt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gvozoxkke.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gjwjdtaxl.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gdfoibacg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glzttvcag.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gwizvuepg.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gudxzauax.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gxzdvmxcg.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxpfuskdq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gvpulfsjq.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gufnzuarf.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gjhluecrv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghnsezatw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gmdeokzpf.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/glllcitop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnokkxxvy.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/guspmhqup.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gdxvojibh.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glewwotup.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxyyuhzdi.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gaguvpdgx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gvvwsxcbz.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gpxvgishh.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gszikzfgt.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gmuedzpxr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/guyxvovvt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gthljylck.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gpcythaqj.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gijhozkzn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gbsjmiidu.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gawatecej.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gooduohyu.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/glmzyowew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gwnxxidin.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gyeyufheh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gzematlhn.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/ghsklhqip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gvzphsymp.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gfsldgtyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/guetfvsrx.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gwvlybleb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gtmcdtjil.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gidxfzbyr.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gfgoqnpuu.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmmwdgu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/guiwnhgpz.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glzwwgicq.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gdqmcxjqb.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gfxuhbfei.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gevepverx.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gejnawjau.sHtML


<!-- 参考信息 -->