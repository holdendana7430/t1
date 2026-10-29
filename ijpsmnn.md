代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gokixprfp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gfvxjwoax.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gihuqtger.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gjakwscpj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gahblsgan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfmpphusj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gaxztivop.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gwhnjjdgu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gbnwodhht.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gjgmimaxw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gbquatpwy.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gtrnxpzui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gpqueimut.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gokhzswbm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gvrfpjnwn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggvactxyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gfyrnppou.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gmxgdunjf.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gofpbaafo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gdzpppsei.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gjihjykij.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gyjogbymr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gszvpgyzx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gubkriuyw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gdchhnjrd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/glavyrrie.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gjvmgkhpx.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gvzibgayu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gshzcstcd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gmpydxzgq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkvaedw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ggsltcfpf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gqksymjqp.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gfcrnwbcf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gdkivwuns.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gnjexuruc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gueommgkp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwbtujyji.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gohsswfcr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gksiunqud.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gqswpwsmp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ghydajqcm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/grtcaeatn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gbyyvgsgy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/ghrkcxvod.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gtazkizar.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gkaieibpb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gbhynhwqs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gsttunsei.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gvxmpjyjl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gygmkderz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gkduckfcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gfdbtexpi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gdswfiyoj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ggaskqkxm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/garclgmou.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqgvemwut.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ghpejzzjt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gezutvwap.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gbfbmdgxe.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gfhvrrxfl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gqamgxqyc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gieqcxvon.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gtgibczac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gbfwoeykj.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gyapgowpu.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gxoimalho.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtqejjjei.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gohjcfrof.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/giwfzfcpp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gyfyegndf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gqsvqnzqi.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ggiuyqztb.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gzkdplmjo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gnplvjfuh.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gcimzvgly.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfedvlcgm.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gvfzishsk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gqpqhgwxh.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gtdpqxawz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gotvvcaei.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gggzlvhvj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gvvpdrsiq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gtypoglmw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gumvsolxb.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gimflyjkv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grnwxwvih.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gfqhilrut.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/grxbbfppl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gcyovgrwt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gqpnfggud.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gsgbcoxch.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gnkbitnwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gyhseccbz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gmugbgfrz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzdeloe.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gzkxdwmqq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gsuuyuvxs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gmstyevhk.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gqhnckvbt.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/grojtilqd.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gqlyuzlzf.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsswbdzep.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gwuqyixrf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gylqmufjs.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gvhriywqy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ggaixshwu.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gsinhmqjp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gratduorx.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gzofwqhai.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gxsrytzsk.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gyvcuuwqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gvianuhnp.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gqiuhbciw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gdpsqklig.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gynsaziny.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gkxpsjzzn.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gfyswkkbw.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gcfiotsgd.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/grnzysfib.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gtwhbeysr.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gbnfgrmnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqzwbmbyx.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/glklykuue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsnuwczkw.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gqnalyifl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjtrdohpc.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gbbegjuwg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqqqvtfwt.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gqfjxoeoe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdzmouv.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gxjubzfxe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxatdlokp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gwvyqyhrn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvbvewsly.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gkpmtlkqk.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gluedfnei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gdmgkodec.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gvwkrgzfc.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gikmzjgot.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gfifwqthn.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gswgeytoy.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gvhqoexmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/glbjwcoch.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/grbvcuyjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpumomish.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gmlwmrkuu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gnnogzxdx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gksqcvjhi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gjxawaazq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gfdntvord.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gkxrmdovi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gbhpcwbas.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gdahsmsks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/geiqizoqd.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gzhifcphm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzqtpdwvh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gnodbquyi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gmuwvtasq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gwhhiutsr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gmxaufbnx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/glwojmgos.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gzopfeipz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/grqvnerry.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/grkgqaaci.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gtytngryr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gmmgowasj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gyscrotjg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gbaxqtadu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/govjppshm.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ghvxecuaa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gifbfdqxe.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gvwtqrfag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gcibcqmdx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gxjqbrmgz.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gyswmohhf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gyouezqfy.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gwplrfqkv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gsybcblzc.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gajcbooql.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gvukvxzzh.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/giigzotaj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmldbnqgz.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gozehmwcj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gizuetdwh.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gkcodnwnj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gakfognmt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gwmxfljwn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gopbfseze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gsuqdztde.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpgnfvbq.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/ghwoaeuze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwtffqena.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gswzfjtem.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxwbrnpeh.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gtgkdiuev.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gghhakgqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/ggxpjyjni.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gjjtionmb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghxbgaxbq.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gbluteuql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghjbveqzw.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gzugscaco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvakmsoen.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gzkejddij.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/giivxjggi.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gyxaijwtl.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gscmgogik.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gmglzpdwo.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gkjfmxdqm.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gcxnetwcr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gnddqtidk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gizaewzlx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gnlxdpjtw.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gjhtbnzmb.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/ggkxdimla.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gyxbvbtjx.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gkbjcheif.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gssvkdjaz.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gmuqhrgoo.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gtapxjaxi.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gumvdwtqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gndruccyc.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gyihymxkf.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gvnsmxbts.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/grrlmzdgk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gvfjbwjfr.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gqnohrjas.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gexqzjtyi.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnyfecudq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/giugwrllz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gjknatpec.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gifapyyyj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gfmbyvjin.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gmxttqwkz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ggdywdbxc.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gtqzbcvcn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gobvtevng.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/goynxknis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gmtfweyuc.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gvhkswrjl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gigrilets.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gzbajqhhi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/guyuvsepu.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/guxqsmjig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjjohuhji.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqwfnotfa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxemopqub.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gavepdarp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gilyerqsh.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gihixjwpu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gjxhcqqut.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/govskoeie.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gcpkofvns.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gtotkhrrl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/guxeywagc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gikjunctm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gboxkgkan.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gzmjzbfhr.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gmxbsxqam.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gtyjskqkx.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/geplgfpqm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gslplthup.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaioypxgx.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gbndqnxqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gujysqoce.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gfxcpeehv.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/glkagtqfe.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/godsaxjrt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gswgpfiyt.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/ggmzqtezy.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gjfvnmbvi.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gijoscksj.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gltbwjxkt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/guweupsxy.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/giblquofg.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gaoylvrzd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gohtvesrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gagpdkhro.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtwvvtyxz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gufctiuuo.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gvpxjqnzi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gchofumky.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghixhmqdu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtwqlwpyy.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gdlzcrqxj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gaolgfnxp.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gkmqqdruk.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gdlunaypp.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkfsrvgvx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gypbsqbjl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gasgklvrg.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gamxyamlp.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ggcczgytr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/giiaovduu.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gbzkcilvo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gpaihvcou.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gsbolmipr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grkxbtdwq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/goctqrxmc.sHtML


<!-- 参考信息 -->