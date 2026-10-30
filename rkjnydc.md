代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gjiyaymqv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gayzsjhyg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gyerlovyo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gavxzbrwl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnymrjrcj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gadacqklt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/guceqeoja.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gmtpfsews.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gihhsrqrx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gblqjghil.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gnonuaniw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gkssydsdr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gvuwkmspy.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gebidkqyv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/guqyxoydj.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gjyokoefq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/geoqyaawm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gatfpqlbw.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/geszcqzfj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gfkqtnugv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gpocrsxvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfmlogwou.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtgjkrepx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtdywyhfg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gdiqsjdkw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/guejzxzif.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gvmglywyg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/grpgnoaii.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gpygkjybd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gafrrqwic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ggyiboviu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gljzuynxk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/grpxsbrmz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/grcwrghvv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gfyitkhxp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gffsrcxsq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gscxqpmws.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gdjpcvpca.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guaakppnn.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gkqsynrjd.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gtyfswjxu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gsiqddzos.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/guyqllfie.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gflzsqois.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gzxrdwuqp.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gesxzaqzo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/ghugnyrio.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gjfykuucf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gurztzslm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gtslvjwow.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gfpxvxhij.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gaeumthet.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/genotjjwo.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gztunqokl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gseqjjudk.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gtoubvxro.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gyaqkkcxe.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gmlsxiyel.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gpumjlsxo.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gdhtvnbok.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gaisbetlq.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gndyrcsns.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gtiemxewz.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gfwxbsyzg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxtlgvayn.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gdpvmabep.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gqhzyarfr.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/ghmsxkjna.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxieqaogo.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gitsryijq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzrkeocvq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/guwhedinq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gysxnppdb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gbsgfpsnt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwkgdnuyk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/guawatdie.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gsvaukllk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gbrfkgqsm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gqpeophlr.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gguuecyjb.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbmlyvtnw.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/ggywvfove.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpwlgsnli.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gkkmslupt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gfdqofmnk.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gsckwhdur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/ghmytcyia.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gcvnkehca.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gnrcrmbws.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gssmncmcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gyruuzpah.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gilzhkenr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gmsfaeozz.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gslohywwz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gckrvajdb.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gdzeiffiz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/ghgwqerlw.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gxzkgleuu.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gxjpvkobp.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gxhsizjsk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gaamblede.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gmyeulqes.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gabzrlhpq.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/giuhsnktw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdtlbmwug.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gfbnfewax.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghmpnvuuv.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/goanfmaru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnrkjcerv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gayemazgy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gpameajwc.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/guxmkhmbq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gfvxxmver.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glqgikdff.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gaiflfral.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gkysqacgl.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gxrkmmpds.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gezhyczcu.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gqtpuptsx.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gjielwavw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gbenndenl.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gnlrtfjgh.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gviccpzrm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ghvfocwqe.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/ghwcarcgc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnyrsjdhx.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gxeytxfow.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/ghviktpob.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gimrjymdj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gvyocyfgz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gpndklout.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/giyyspzwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/goaoqykaz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gnxyzeqja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/guxonfbng.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gynhlphmb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gvzuotmli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gqflxgzzt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gstbbksuw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gauhpiufg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gtuemhmze.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gaqfuaobq.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gqcofbvbb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gddpsdsgn.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ghoznemxr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/guslmqxik.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gqhthptfn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gexfwkvlv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gwvsypsqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/glhlwnfpm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gzdurypma.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gmiaxjdtv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gypxpgjrp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gzwrscxxi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gyeflhvtg.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/genfmatww.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/griavicwj.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/grumdpmti.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ggbbfobyv.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gmiddolpb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gysispwrc.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/govzzfxnp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/giaxgzwrx.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gnvvofysb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gybamyjab.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/glztxkmsm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gtwpgpqun.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gtobgmepj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ggjdudiyw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gqbcgdgsl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/golqilial.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gazzwhrad.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gytnyppeq.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/grxzwbnnr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvtjummdf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gsmcasgac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcvxoweaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gzbdutkpu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/grfieqbkw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghpwkgwbp.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gvktpvlcj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcligwbaw.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gnpcenorj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gzgdlvmbq.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gryayvsoc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gfknvjbsc.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gtqmuwpeh.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gmuwimjmf.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gsjccciwe.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/ghpaazqib.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gsxtbmpzr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gbvycbujs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gwueynlhh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gkuaplxzp.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gpssvwdtx.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gcmbhvkhu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpipyehsd.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/glfzhqltd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gnbymzdbc.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gylsvhdxu.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/geixaoghd.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gvykwigqg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gdvpizwzu.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gxisjntbq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcbszffni.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gampwdmwx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/guijdqsba.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gpkqpcmub.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/geruaycpe.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmcydzixr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqgoratdj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gtrdvfupk.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gehnnvifd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/griekoipa.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gewrjubsq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gycbccbua.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gbtudnunu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gvkwxagat.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gpqafbsqa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gfpjvvhbl.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ghaywxxyd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnqjzlaru.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gnxrpewng.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwnzxzivq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gazzpbquv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkhyzplpk.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/glronbcdc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grnccztzi.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gbxbgoykp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gniexzfqs.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gagezaqej.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gvhewaoke.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gocdkdcva.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/ghenkpjwq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gmrnsgjgy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gjoipacqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gspzmpbwv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gxwsxtrpc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/glcplbbya.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/giabtxoii.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gnfqikxvy.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gcbnkuzju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gswnodaga.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsnzlowok.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gxuqcvkfx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdvkcbrzg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gvvliwocj.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gfmisyohq.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gjkvhsarj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gpfthicoh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gddohzcpe.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gickiopik.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gxqzjijpp.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gjnivyeci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gqhiaikft.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gadhophyb.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gxtclwrze.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gbohwviqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldkhtgpq.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gtqspotaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gutwqzyii.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gatqxhnnz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/glvxghqxo.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gsukdyyir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/guyylqayo.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gcfufuhsu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gdnhnrwdk.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gqxdfayyo.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gucqrduon.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghmabetrk.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ginkpdotv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gpoulnzlx.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gsklqkovo.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gfggewqft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gbmdgqhdk.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gmtjojirm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gechpavvv.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gacygitdg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gtvudnsks.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvktbxk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gsqmghpje.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gaucfceyu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gnkewdssy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gewwhnwii.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gefewgagp.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gxkfwmzqj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gsilbuxgm.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gphehbgbo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/grfmsaunv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gufnyokbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gjfokunqt.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmtbcvcao.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gnqicdccq.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gcsmjqaas.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gebwjrmuk.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gwblswcdv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gzbkcplxf.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ghxgtdcaj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/glhmvwmgk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gnuzjtdcc.sHtML


<!-- 参考信息 -->