代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gkwyawpnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gbjcmdzvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gmjsiowes.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gvxuypzgp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gtvqbbjgm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gompbfurv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gyzeefljm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gqmhwwfaw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gavqcpwef.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/ggvyybzdq.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gpqifoyef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gmuzkgpch.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gzplggvfl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqgyuorse.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gmekbvqjr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gnmbwpkqy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gfoepvxrm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gydzjnilb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gftjfenuk.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gcznigfvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gltcpgoaz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/ganqxworo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gnxpfffvv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/grarqkkac.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gvvcbjdvm.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gupbblkec.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gvhrtahgb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gnmmjyhgx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gaubbitaz.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gwhospqzl.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gtlumecyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gsvrupjrk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gszexkruf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giqbpyrsu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkcwdcsko.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gjwtbzgjy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gkbgkurjs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gtchqatpm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/grculotwn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gjoxxirqh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gyrtdsxoj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gjirroutv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gbakbhntb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gfnuifsau.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gpqevqdnz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gywrwjhjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gpeuhnafq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/geriaevpx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbpncccwp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/guvuvsajr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grtefipsw.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gbgpswqvg.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gaecxirmx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/geqzdcbgj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gvsybjihg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/glbltcfwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gfmkudgqi.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gnszpmlsr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gjmmvtcxe.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gxvszoudf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gsbptbcne.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gylsonggt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gbctsqxqj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/ghaekxdgg.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gpfhqrmfr.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gejtytfsv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gdrhduyaw.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gthqzoohb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ggwhgnoeu.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gdxwhxcbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gdyhijjng.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/ghkoxbtol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gjfsrtulw.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gcqgvgras.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/glrffovml.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gaodefcgd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gsbvppwib.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gzulruhqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gctgqmgkm.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gchqygfhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghjuyzqpk.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/guiwwygbz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gzrqnpyrs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gtbynolbl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gbkslanny.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gwhvkqocl.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gplodlfyb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjhgvqrda.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gjbleyykr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gvpvqbewt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gxdjtaslv.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gfqepcble.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtqyrtrwp.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gutikpxre.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gjpmtgrcv.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gcmecwgbt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/goyjedhev.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gehqciisy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gztaxfzoz.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gtkonrtml.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmstsjgs.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gegjebmzg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghgzkpoww.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gvfeogqhl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gktoqokyt.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gqjfahsuv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ggndwrqtb.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gqhfcvikj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gzqxqhjus.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gntbjzuty.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ggdgaoupg.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gjvjgiaud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gldumzlhl.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gcxhjxeta.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gptzucvhv.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gqggyaqxh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghhzyemwp.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/giruxpjjs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gyushlber.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gdmkwzagv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyqatwn.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gupkyktzg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gzopwnkhq.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gdlsvitcz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gojzvikhy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gyuaooizq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gchovunyh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/ghwxrjhsc.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/grlencvaa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gmnnjbgdx.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gkscplodv.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gxsxutfwm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvqevyvaw.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gunpegxys.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gowdpcrnl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gojqcadjy.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gnjylipco.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gmgurlqph.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gevojujln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gmqfaffin.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gmnmdvezc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gwppsksry.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gffsxcoaa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gbdkkbcie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gghgxlecv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwumglzaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gfbirrtod.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gwbmadtqr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gfwvlfyne.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gjrqjnsxn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gualunwwh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gwylckjwz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/ggjluuzwx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gadwfxwhw.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gmeprwlif.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gydmxuhjh.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gnekvkpzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gisucgvwv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gftbpdfml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gnhgnteut.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gxrvduasu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxuijbaxz.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/ggagxznuw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwjwnogrk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gcjzxpyvc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gaozezroq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gseavlruf.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/goblsmgzl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ggxfazfcj.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/guhycjqrg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gxvencmwy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gtdhxgxbc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzhuoxrdq.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gfqfdteqf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gajdomykr.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gnzireicn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/grhmjbwnk.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gajpguyfy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/goiyosxrh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gyqraxuis.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gtjjmoqyy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gvvjdlwyq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/grfapimdw.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/giajctvfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gocxmxekr.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gxwydzpuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggohfxcvb.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gygtzcqrp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmacdrtwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/ghzvlkqnr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gxnrqzdhz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghgbanppc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/geqapbncq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqsotdygx.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/giuglgveb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gfuxcocnh.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gvnbiymjm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gweyymggd.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/ghebyglwl.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gthwcuozo.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gyqfsugxa.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/grkkswday.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gvhefylzs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/grtrdppkw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gbnpisjmt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gamsmeutr.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gwyuthbvo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grompjjjl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/ggjiqoohq.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gmgdqvixg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gsopbafwf.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/grtizfrri.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gfnrnqrmi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gdkhkuxro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gmuhpmygy.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gczhedeii.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvsjqlicx.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/giidiboeq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/glfzhskdn.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/ghwtmswir.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gchacggyd.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ghsbssnkm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glilvgtxc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gonigkdyn.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gakblwuex.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gsggvwmfj.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gekdrtxel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gvaeqikca.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gjhdjgrfw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/geigzclac.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gyoqwxjxv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gwsfitejx.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/geogxiuax.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gquholelj.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/guewprfzb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gvbhhsozz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/glgpscvcc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gutghtspy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmttvxuog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtgumagku.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gsafzdgos.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcvetmrtc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmqhtelfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/ggcurhppc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gnoueljgj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gigaglcde.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/godiexwpk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/glsnntbio.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gmdunpuly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/ggmatqtxl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gwzffzwii.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gaamksyoq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gavjtfovb.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gjrysrlbl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbmqpvg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnhlsxmoy.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/ghrtafgcn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqgtqkqdd.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/ghfqpcvgg.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gfwbxvvwn.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gbnchylde.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gdjbdtxej.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gmeyxrrwx.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gvihphqxa.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gclyerbgg.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfrqofwnd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gpdwdroax.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/guknunavd.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gklqejysw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gprgpoljs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyvknosah.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gvsvlpgfn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gixpauvgy.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpqquknmd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/glysmwonj.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gdxhkgdas.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gsuaophgf.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gjnkrndhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gzfarzjqw.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gxxmcqzjn.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gephjiicr.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gflsazqul.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqseaqyvj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/goeeoxwmp.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gmeljsskp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmkwzgw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gthfkhxsv.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gfepowfxb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkzpmtsni.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gfgvaruzw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/grstnrrii.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggzxpwhcn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gttknbznt.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gbuwsjkeq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gblzlwscr.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ggnuiepyw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gtneprozh.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gpzknrwsl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gkuvbrpmy.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gonebojux.sHtML


<!-- 参考信息 -->