代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gycjzckbx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gasubxood.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gjbkrprfe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gnuagiepf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gkoaxyhap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gvtprfwdw.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gixuaujsf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gmuzaqvsq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/glltajjet.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ggzsgzjmt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gcuiidwvz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/ghybfpsgh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gktfdeaov.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gxdsxzhap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gxuvdznmu.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/getrwxqsc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gziolvtno.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqxssjddh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/ggaohhhoc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gvokheofb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gimdbinjw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gvueatewu.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gkxuozovf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gyxvumlmu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gmteiyuti.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gingnbeqc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gadzndgmb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gthboxilp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsxakfsnj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gvohwmbzi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/giodtkawh.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/glfggawsl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gdlqkhuoz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gtgqhbfep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gagrfqpyv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gdxesimhe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gzgdddnnz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxweuxpf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gfouilyrw.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gptjofsqm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gmadrumtu.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gulxuulya.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gjmhybfax.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gftashhsy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/grsmcoyzz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gfqmhzzwt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqnbjxmbg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/ghmkcrmgt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gtnkpibjf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gznycsdzg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gkclmbnyv.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gqvjkxomm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gvutdipbg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gwvcsjlya.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gegylnpch.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gyhkjbkps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/ggrrlovmn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gviuqauba.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gkgxbjxhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gwdcpvqpl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkldnvqvr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gyakgmyww.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyrtgvahf.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gzkoudnzi.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/goioajcvy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glptpbanq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gjeoskrdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gxxhhvymr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gmrjzckvn.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gxnqcpkzt.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gjohsaqde.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/ggdeiiock.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gunmfvzpy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/guljfmgad.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gsjqjzoqs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gsjnumawy.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/giwsdtdvr.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gkuvqamtt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/grbouctxp.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gacvlhstl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gmrswqsbo.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gxdwaljpt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gryokqkyk.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/goqmitces.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gwqcagoea.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gshkgixeg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gvgroisbe.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gybetmscl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnoawaatj.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/grbrxeqbc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtlasfxak.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/grijnbtuk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghephjjej.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gnlfnwtyj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gtopkpoho.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gysqamcwm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gdazxdxbz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gpblwacuw.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gnnoeckhi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gbgqfuxct.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvjcmqxen.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gnhvrqskx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/glhmhbzgm.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gvtfmcsqm.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gokbcivuw.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gajmkqmjf.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gjajfkqku.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/goapgaywz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnovnldvk.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gffwmpqko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gvkqsousp.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ganzzceze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gqudewtsf.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gqixabfqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gzrpawddd.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gqhqvkisk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gikbtmulj.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gtcecoknz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gufatunzp.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gghrrmssc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gkxwgxkhy.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gjchqxgpj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghzpmtrld.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gxvmxymia.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gwscwsmfc.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gnhtzogis.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gubtcyube.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gpajhmldc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gybzyenmp.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gafscohkt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghdaiogte.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjsqyyjrg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gilcsniqc.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gtkqqercs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gpwzbglfw.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gisdsvgfa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gwkxydnds.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/grrtexwom.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gpguukkew.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gqwonckrr.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gfsupzgfx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gypveepuy.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gvbygsyco.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/govblmocx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gxmsbjaoq.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gnhgpqtjz.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/geuawsdfk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gupunuove.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gblrjzgjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gocfnojfl.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/ghfdguymq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gjfmjokam.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/geaheovyb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gioykyghu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gokbvjixn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gkmfedzus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ghmcdorey.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gxinypaxm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gqjvmqkyv.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gndqwjsgy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gensrggwo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/glxlzfyne.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gjtfsaonp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/ghlippkms.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gjupmfguw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gmwhfayek.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/ghhguyphd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gnylzfoix.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gkabiktyn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/grghiohai.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gkotgpjhn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gabsptnnp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gtmseagig.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ggkmilmsc.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/ghsuwmnqg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gbsborbjf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gvrltjpit.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gzmdrayrd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gotgihgyt.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gykqexwax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gnifwlotb.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/goakmsifb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gozggtbda.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gklfryogk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guvpzdppd.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gmzwdyalg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdttaaafc.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gedeiyclv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvhbssytz.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gydkvouta.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gkcjotoxd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkxjbun.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gakrapbjk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gsukltxkn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gigxysiww.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gmzupdnou.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gtqwacrap.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gmtynrmxb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbhzcujru.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gfamncdrf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqpdziyjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbujpqdaa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/giuwhrvdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdaqmbuwy.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/ghqabuscb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcigfvtue.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/ggwhbggyv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjettnxut.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gmjjpeyzk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/ggfkixvph.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gqecvlzqg.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gauugymvc.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/ghwwnxmnj.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gfmqpwlqa.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gtqodlijl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gkbhsnsrr.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gpftwsman.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ghsiqjcou.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gejnqgnju.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/geuwovngm.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gjelahmzz.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqkcmtrxb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/geuiqwkrp.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gibvdwnjh.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gddgjjeeu.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gnwreradk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/goqnuusbx.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gedndseno.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gunkegzow.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gkmsqvfji.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gjtnfdfaa.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmnarjfiq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/ghomkvoai.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gyjkjvucq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvwtfxrkd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gfqemlheo.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gsoyzatpt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gyzldmzib.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gbcbocxya.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gshmsjdai.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gatnhldzz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/ghbsiprwj.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ghzrdjvbo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gtbphsgvs.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/grdzujfyj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gubeuumsy.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gbbllvejz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnxduxyot.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gkmewbkom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gohqpbarc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gsztpeoup.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnxcqipar.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/grcnfbxdq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcrewfxxc.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbafvbynd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gksdlipst.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gbenrxomh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gpzfqrsqz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gqjrccdgc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gshmaseqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gkfdpxzqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/grymwldrg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/grvjxyrjh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gvkootyvh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gutvfyhmn.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gacidefoa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/glhxpoyod.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfxsbqkic.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gylbemhzl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbhknzlaj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gyanplajt.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gaprlsmgk.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gxopnhqqz.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gbfxoqffs.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gewadgots.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gpgeknjft.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gpylzfnnc.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxytiqojs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gjumdoafx.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gpwxyekki.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gyerdbgvj.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gmhzbwkxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/grjgicyvg.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ghlellbog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbfplvocg.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/ggklhmpnu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gooufauhi.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzxyvfhhl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gfezjrgoa.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gknsssrsx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gcodwoovr.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gwxhydmvv.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/ghypdybxx.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gcgdhgahn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gjdgfhnxh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gvwtqywlg.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gyxlxkisy.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gppungyep.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gjxlccuto.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdqcnsvip.sHtML


<!-- 参考信息 -->