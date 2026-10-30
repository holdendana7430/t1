代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/glwilrpds.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/ggicifluv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gkeymktiy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/grblzmbtv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/grbmtpnlx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gljtzfyfb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gmflnddtg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gwnmzizaa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gynihxxbf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/glwcfatym.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gwqlembcf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gqdxaball.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gyoiwtyio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gvixgaxsp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gtpwucgvp.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gcbpbhglw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gpkjjijqz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gcljqmuec.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gmuddinci.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gdxzjzpag.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxohmzaph.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/golgvhxfq.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gkuoxfidd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gckwbloig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/grriyhmoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gkpwuwahv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gekotkhtf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/grxhubawz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grakxkxjo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gddexrbjd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/giepkajfy.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/getgzxtxg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gzqwwcsfn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gntnraqcj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/glsfneujd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gpyfwmhiy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gmsvfgwyk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwxarlwvg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gokhebmpp.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gogdjfmwr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gvzcyudsm.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gfexvmdmz.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gttvtjtuv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gwizuqcnz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gknodntop.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbzvmjfru.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghwaytecl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gsxydggnv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gawkakvdu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gaewbloka.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gorfertch.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gatusvwlq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gpkasoauo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gzmugwzfk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gmtvgzshw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gvakrytax.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gyitedaop.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gjthwglrm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gzdzwzdwy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gerdjdyyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxzddugzu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/ghenpjhcb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxkuaayqn.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gsmxdfmod.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gwiqjvgie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/grgfrhmox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/guotsngtz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gofdlrciw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gqwhuzwob.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gxqagmcfk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/ghvlheauo.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gxykjzead.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gufiaterj.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/grfnixfxh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gbavuayyk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ghorojorl.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gsducftht.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gzfksfevb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gryzbohgw.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gqjjgpjzr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvvqrcruh.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/ghlktqxgx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gaopaiwqx.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/grcksbnwe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gvtdyooxp.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gxkxcmxvk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gzlpktcsm.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gpfdhkplh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gepxnjmot.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gslhddgvi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvftxnlvn.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gugfnvbly.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gtyquifbd.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/grikxgykt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjmfnqsuw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gevzubxkv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gjsmjjinm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/glczotbrb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gymkwgumb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsogvthfq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gljlrrvwd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/goluzmbkm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/grlgvglsq.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/ggbpbpkzt.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnajmkltp.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gikejbpty.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbpoyetxu.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gxgpwvzfd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/grwvlxciw.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gcxxfvrer.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gymmjbdjz.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gexqwhvso.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gkxbpciho.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/grpnfppou.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gtocpdalh.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gltkpihyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gdygirsjg.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gmttibrjy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzntoku.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gkrexcxlm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gnhrptswu.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gtvoaqqay.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghotpbqld.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gdyprpymi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gkdvfuved.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gqygqiwcp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbfrmbivj.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gkrmaqsno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfmsaxutp.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gutbwnvkf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtvwzlpvm.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gtquzcvps.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzdxywwse.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpdmvizlt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gmwzurxso.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gxxobexan.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gznudvkjf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ghgovacti.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gddquoxtu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/glhmlkwnk.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gugdypquc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gklplfeeq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gvmhwxkty.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gdemnrvyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/guegfdvsx.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gqtlumjvt.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gnrjludez.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gblfzxyru.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtnibjryk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gtrohutcg.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gxoalinjl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gvmvtmyye.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gtdwzcgat.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gwmcszmrk.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/grilgdcma.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gahktjtpo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gvvfxyspc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gjgihbmki.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gtgjogbmx.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gnpcercvi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gyptnijtw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtuvvgxlv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gqcpfawzq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/geunsobat.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gtedxtaux.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gqwnznhvx.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gckyqqmva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gamhspwxo.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gmwcfyujp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gulqatwzk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gklbcdwwq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grrhiqeas.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gtmfoocnp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gphkwxtml.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gogysnouy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gbluibglf.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ghwvnradc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gwzjyjkzt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gjyogtznn.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/goztttmbr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gqltwkrhv.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gzagargor.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gbmdfhieo.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/goheaajbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gvptyxkyt.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gaxlfvpgm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/geswmqlgr.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gnrdpbmha.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gboirdgne.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gclgchjws.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gfgmirolq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjvzxcmxh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gjnkekbdq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gdefhltue.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/ggigefimr.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gymsdauvr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsjkihwth.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gmtnyxspp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gygzokixs.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gnpzldauo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gegjptdrv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/goukzbvys.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gsamzeros.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfipxkcxl.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gvpmtprgq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gosucudww.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gckkiogbo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjpflpuee.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ghxdclrxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkebram.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gmqgcqzle.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gcaotgvai.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/glboysycx.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gyvjkasfv.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gvtnprwcx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gjqicqjoz.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gbhkmqbgc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/guqcxqmou.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gdwtrfdks.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gdeffmmul.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/galdqfwpt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gzghzdqkm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gdvdzqfnl.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gcmspokju.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gwvhfcwya.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gcmbgpowh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/ghyqqektx.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gtnghbszl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyiuaafvk.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gmtltyrum.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/ghsovkvvu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gjilhdrcm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gqcryohhw.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grmcfohdu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxmlahsfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gxzckkjco.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gwycwwudy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/ghlgqtdhu.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gneyrnsja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gqimcesvq.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gzbysmnsb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gkjtxfjnl.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gzrooebca.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gwxjveprw.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gxowpfkck.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdjziuysu.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gbsucgqyf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyjjknrta.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gvfvkxlhr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsmltuxwn.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtythxnmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpldljgdg.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjdnscqaz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkitjlzod.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gqwbubjxk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gcuzkqsdq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goozafjwv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gyorafcre.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gvhrwwhgm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gynhdxwfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gedimesbl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/ghzrphhjq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqnufqyew.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/geoygnxkw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gkunrfrzn.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gjptfwzux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gpwluadnu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdstfhruv.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gobvwgyqc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gctlnzvju.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gzfsgojpp.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gvmbtdexi.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdxuatzrm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/glqrmfjll.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjwazqjpd.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/glskqwfub.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gvjdmxwsi.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/graagqckq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gidfjyyif.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gyzicyomh.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gqpghytza.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gbvlocyoe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gydvhklvc.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gsckydwbq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnemdixna.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvdyhjqyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/grdbjjpbf.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gobfhafwt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gvvyjkzlu.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/goenjwmbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gvtussimx.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ghgquezof.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gvoqaygkv.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gfjngyltq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ginnkvkds.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhelrnjp.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/grfdmvsdo.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/glydawmat.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/goatnkwrw.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gnckrcghi.sHtML


<!-- 参考信息 -->