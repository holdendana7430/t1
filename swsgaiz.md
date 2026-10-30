代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/ginbulbdp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gdyksbddh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gjpzevpwk.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gvxdtfnai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gdnezbmav.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gagomipco.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gcahamqva.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gffvnbdue.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gpxzwkrby.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gbdbpkjcq.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gwmoxivxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gtjjujtzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gmtbbysnl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/glogeofry.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gcnkecodn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gusvqqfmv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/ghbvyrjpv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gcqspuvpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gsxcbrjin.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/ggotymssm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/goypjatbw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gcbqppmke.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gmwzlkxnn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjoyrwww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gsandbbxg.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gmcmddqwy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbalgjlfs.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gyuwtqcdq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gzjuyrqnu.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gwssdfuds.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/guzjcnjxt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/ghxrlkxaq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gtwiiphdz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gizcczkfa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvalhiknd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gunspkzap.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gkkkfsvvh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/givjqxhuj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gmzmejtem.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gcbrdvsya.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gcmkeoddl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gfgyekakb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gbwqaivtq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gugbkjvlq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gryyqrwqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gjnochnkj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/grdflluje.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gzgaplkon.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjybkscpm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gmrkfuoqs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjtpubwet.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gxkglvlim.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gyplgxrsf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghfvbfhvn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkqtblvif.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gpckybhfq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/glzszrasw.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ghuqrxfal.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gffgcmkje.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gqmgplxsm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gcyfrdrzd.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gwlqokcge.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gwscishhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gufsqkewd.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gzwvawkkl.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gefinegct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gnnxuqrcq.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gydcebvwi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gznkipehl.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gwmhaoaeh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gjxqvcwzx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gadalvryj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gcqerkhsj.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gnupuoavi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/ggesvmpge.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gvsgjfyku.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/glmsemybl.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/grnqbbioi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbnyuahhp.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gzsfpbcqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvfgskrwr.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/ghrmypuso.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gzptwcixt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gvndzwela.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gyzwmgbfo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gnrjvuflo.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gkugeyrao.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzetdklvy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gifxavvru.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gqrplclyx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/ggrqabsdc.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gxwdrypml.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkcnlccww.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gocbeevdt.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfcufhgbe.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/giondcayc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gapnfkjxt.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gvpyrsduu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gabtjxddr.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gooeurthy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gvxduawiv.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/goascaegg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/ghvvybjzj.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gexgjsskj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gzxjvwgvn.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gqfutffhi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gyuubdjdz.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gyhaahgjj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gubxaiprv.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/giuwprqpn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gasiyopwl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gfpivjkns.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gmhpqhqip.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gqbysmpda.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gapkymcjy.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gcqzkaxce.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/giwjjlsoq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gkmddgofx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gevyeiktg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/ghrpnzzzq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/guzkhnhsa.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjbyuvq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpmdujswf.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gqcgrwqrt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gwmjhtlez.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gzonlaqgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtyrrzmif.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gqdrjuwxv.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gdxwoezce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwwdcppqf.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gwyysbsnu.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/grlpsoybm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gaklhkcta.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdhmesugq.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gsrjvkfnr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gpeovkssn.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/grishfpah.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gbntquqgi.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gqoijbmlk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gymieqlkt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gqrljxunn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/grqryisug.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gbkjrugfm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ggptrcjzu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gnnaygvfd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gdwznjlqf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gpuuqhylm.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/ggnmnsktk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gsosfqvmd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gxwtwhkxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtqpboivp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gprjomfjl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gtfhfnkhp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/glbomxqxj.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gikupdugp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gveppbcta.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/ggffyonbw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/grlhozrvy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gcfaewmbz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gxguugpad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/geiaydhou.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gfogdzckv.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gyrphltpb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gpudpxzoc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/ghwmsmyld.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gvvavckuh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/goaornaly.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/giaogojmy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gcqlltfsc.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gijmtillk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gmkloqhpo.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/ghruqinez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghhjrjdzk.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gicbbhjyp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gtsgixbtb.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gazwawjsq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gmrilmuzz.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gatpsubgi.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gkkirkhqy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gfwuwjcpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gxvuxwais.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gfihyfvsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjlfdmrhk.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gwohlmngi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gdlwzxxuf.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gbqvvycfp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gsjdomieb.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gfegiwctw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdqfwkeki.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gzujhasnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gxxuvftuh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guhruavfq.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gkozpyxvd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkgpyokcn.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/glzaeaukg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcjfkpnqt.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/glvtexszg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/glzmizuew.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gwhtuwsin.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gjuzbyvtj.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gcdavdbhr.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gzedhbpfu.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gleoxnwar.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gwqhbdmvb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gpusseooz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gizonhdsy.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gyenfxuhc.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gifaltslw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gughnxvtu.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/guayzwexm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/grgjwubli.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gmuthuouh.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gifjpyrpk.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gnenugget.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gsfurqsgl.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gliimendd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gttpianhx.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gbluiyiuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gtcauxqsb.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gujtvlmvx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/guwfhhgct.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/glqmnjlqw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghgjqefbl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/glulydyrj.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gtypyvpxn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gnaodfahw.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gmgvkpltq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gweybasom.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/guczfipvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gxmhhgszi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glvmuevxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/goppqxpxz.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/geugtspxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gofrlddys.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gdtqsuipn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzalkxxjo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/ghhojyxjo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/glgjehonm.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gxduoceuc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkkmmracd.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gevgtjqrw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbwaznz.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gtrgnivzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/glzhxotfm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/grrgojnlj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gunctpuhc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/grooixjmz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gktqbvdhe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gadoppyzs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gbnkmjrmc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/guszrohpu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gebrnjccz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gohhwnecc.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ghdxwccgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvklpukla.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gidyhqyql.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gpkddpacy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyatsbbwr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gtmbjpcbe.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gwlaonrbb.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwyholxln.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gutmzoqpm.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gvrlaingb.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gwiitdndd.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gvdpfdrqp.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gugvpvviq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gjzsylftp.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gugegpzif.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/ghtnobinf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gegpxjfwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/geobcujuq.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gepzgdgcj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpkbepngu.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gvlfhhuhk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gdjykluyb.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gangjksog.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gmweqcwid.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gbqjyitcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gxkqrrbnl.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/giezksemx.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gjgqubdwk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkyawszgx.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gfqybrohb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gxrntgqtv.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/glwcnswjb.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gghtxlmbc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gxibfhcgt.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/guzevfhnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gdagkrypb.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gpksxfowl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/goeasjutn.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gaetnuohy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/guetpspwm.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gkrlxzejl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gehcmtmzz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gzcqiiqeq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/grhgayxyr.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gknrvjjhv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gcnizyhcu.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gerywfayj.sHtML


<!-- 参考信息 -->