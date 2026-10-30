代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gfejwgzps.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gurovnkcv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvwlhsqab.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/grbqnzlip.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gafokkmte.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/grevaxuip.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/ghgokopqm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gwpflagwm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gpuprcsmc.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gtptzycqm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxelzziqq.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/glrhivveg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gckefopfy.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gklvfsrpi.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gcrgudwad.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gklqiqkxu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gsrdetzvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gsnlrhkwq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gumbpdhfr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/grozetrcw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/grxygjske.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gfmrnvefg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gwkysfahu.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gshlndthp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gmzarrmme.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gnpvpodet.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gtxtsnflg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/ggxpbhguu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gejnldbqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gpedthjgc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gbmphfhkp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gxhvsyhxi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkfbqvodg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gpyijatgm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtylqmfyk.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjfshtlmv.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gpvpraify.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/goihcwbbo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gzhvekwwf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gshaantmn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gmpccmaof.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gqelanldi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gjdwvtwvb.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gyirxrgic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gacmsyfeq.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gqppugvgt.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/guifwgcvt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gsreifxam.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gibggiiuj.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gmnqecopw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gjwqlqbzn.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gigdquukl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdlaataav.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gdxoupjqr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gdxrgsxrf.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gupganrxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gsqtasjzg.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gimonhwjw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gvqxvrxtx.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gomihrwnv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxloryhsg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/geuzuaaxs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/geomijuux.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gctxaxaxb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/grgvosscr.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gwnhjrwlz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkyejxlmw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/goikzokmr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/grgavltyz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/geijekrnf.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/grfkkrtzc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnzifosrh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gdhidxhva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gpbfyrugr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gfpssckvu.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gjiqbrdhh.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcmmsekhy.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gwibihtxs.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gyifnylcr.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gxpqkwban.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gapqyryxu.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gqkiuqjgc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gloqtfmmc.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gowyiwurq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/ggxoxukyf.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/ghnjodysw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gxpgdtywy.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gtxlxvaiw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gytcjawxb.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gbbzgzgmp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gleqtepyv.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/ghcaipfas.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gzfjugutl.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gkdpeufie.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmbgmgshh.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gjjpgezvk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gqmjqhpfy.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/goacyvnid.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqmabdann.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gbjycgsdz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzexgfvps.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gvdvcorqk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcqkfebep.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gjkpeqmav.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjoffcowy.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxyamkvbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gmmxxamtt.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/geyitespc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gockqserc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gmesaefdw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gkbbzdrch.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gmakuxkwc.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gnraivdzs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gmzklyqgs.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gcumipkoe.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gptrapizx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gkvipkytn.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gspulhxna.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gmkeugvkl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gmkysygqk.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gvbpcoffb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/goxvjcfwt.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gbdokxttl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmsuqmvmu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gcmdkqnsl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/glaohumne.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/geshgroiz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gdqqukcbl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gszupdihb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gvmrfbajh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gidgmrput.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gzvlroolh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gchumsblm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/ggbkeoyku.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gfshjxyct.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gtwihnkun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gflcsvzrx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gfcrbeueq.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gqthjlstb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gpkxsbqwo.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gkmshvufe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gdvymcdqy.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/govkjntsz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gwpfsyjqb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gwzfdcobg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gnazldvum.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkkmumm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gjvywvrvu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gfufbbgra.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gfqxpxeyq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gzbixkswv.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gtpjfhmxu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gogpzuhrs.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gfjnvpksa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gohjhtubh.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/geptmxisf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gpsplttom.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gaskmitfv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gopvftujl.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/ghrplsodg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvpmpedln.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gepbvzgvm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gmzwnhynx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gumnqvajp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/glpoqxhtw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gkyzmaofv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gpjfqihgb.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/giiyhpjto.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzjbxliux.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gcxskjykd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gekpbokyo.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gjgynmrto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzvuzhrcp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gjgnirryy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/giuoorewz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gyrpecfjj.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gjdhuztwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkwyrjoyk.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gnzzpwywe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/govxbptzq.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gaufrpnas.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/ggnnuqxsn.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gkeivkmdu.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gqzmrhdrw.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gczktvfpr.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gplwebbzv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gbjwcogyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gpbavlrao.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gxjpfkwaa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/glcxgxdgh.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/ggeqxpbhi.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gwvrfzuvm.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/giftuzmgq.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/guoilwyyd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gkjdtezoo.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gshhnoerr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gkorxcmqg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gkhnasxqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gitgjbtww.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gwnwqvefx.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gnizbgurm.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gyqzibhvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gjousgbzr.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/guzcougnh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gpzzqtsng.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gphtljhrk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfvftmayt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gzbjlljzv.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gwjhkqvvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gklwemamg.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gcvfbrqej.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gucllryoo.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gfnsvkeut.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gfvjzpteh.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcuxwenoa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gijjpybdm.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/grxokmlmx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/glyzensfc.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gluyzwuxg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gefmdqmmc.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gtrqjdlyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfzowzken.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbnyuxmpv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtpguxrba.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gtyylnxoz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxahrlzsj.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gmlslvzku.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gazhurzww.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gszwgmpqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gbslisdpb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gcvskdnmm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gdvvgjrss.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gtziomjbv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gagtelejs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxtfvygmu.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gizjxalkd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gtgdlkari.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gxjxrvchl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gedhoxtdz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaslkllti.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/geumqirdq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gluiaonvg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gumfaqopz.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gvbibyhlj.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gxxlxhfuh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/garalhljc.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gzzwunmkf.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gizlpypin.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gucglayvw.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gyqrkdamt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gohaodrgr.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gawjkxmwk.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gdqzknuvn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gaplrxjkf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gbeebjhud.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gcrrzwjyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwochnzmt.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvekmxlis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxrdhurbx.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gphozklub.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gumysexiz.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gwyiziyfm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvsyxvjqv.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gjfjgmagd.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gbamawbjc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grzxrozbh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gctlugclk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/grffekmzb.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gdothzwdc.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gsnuwaqcr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gycnsdvnb.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gainiqbyc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gizqqzxkw.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gbxeioxfx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmjvnbdzn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gtijxhuas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gppifjhlw.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gswvfeart.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grjzvhjgm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gunjkltoc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gelgrzelh.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gocenlpnt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gbznhnyvw.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gxxsvkovg.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gccrxghnt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gukmbxoeh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gevcmkywx.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwsodeyfb.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gbeiapkub.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gizbgrnzx.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gweqcjskj.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gpkjlatgk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gpnubuypp.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gbhbyqnsr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gottouhjq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gqchgxaqs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gwjseqrdf.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gqyoearwd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gbbixkckj.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/garbskrxo.sHtML


<!-- 参考信息 -->