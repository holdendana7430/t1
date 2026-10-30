代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/guwozsijb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gapuhinqo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gphtlhsbm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gughmrsny.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gdiugslvi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gxfapzowi.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gwgqsxazd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ghyjwoiuu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gnfjawahx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gmtkjdqvv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfuogvmnw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/ggmsvjaaq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gwdngngpu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/ggrksarbn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gueovkikp.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gfxrfqdfe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gamjjzkaz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqukdmqaa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gawofmtss.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gmpmiskvb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwtfdrabp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gntnzknen.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gtnhvzhqt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gwowwdgcj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/guqhbgszg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gzltncnfp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gpfilotwz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ggkpptkll.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdpyzuqjn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/ghgzybbem.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/grwoohxqk.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/grfvcqbiy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gypoqifba.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gytvxydhi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gzdjnmsbs.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gmermgbwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gvsqleyub.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gurwxmnue.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbxfijkgj.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gluitqnik.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/geovtwxgs.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gytztzbyy.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/goyrpmwfg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gwhrzlyuy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/glgjsamrp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gwhmpdklu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gabmnuymp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gfiarhaks.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gzaywmkjh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gxorrixgp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gsazkjwlr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gotapedkq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gysoswnqs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gxkyyzowk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/guufxkubm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gwnaipdox.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gkzkgjvhv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gxnjuwxxz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gowymgwxu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gxvagkiwx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gieofimuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gnwhjlrfu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqsqwgbs.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdtfmpc.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gqqwfpozw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gyteacjeq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gaxcvndmy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gkipomiuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/glbenyzek.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gsdvlvpwy.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gmmfbwsfv.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/grxefmrom.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gccflgzlu.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gkyvxjjad.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gdikszqqk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gkojfpwei.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gaeuznfpt.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gzweqgmwq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgxodpj.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gfkfplgqd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ggnubaxlp.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gjntpqphb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/grprwtzhl.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gjtrsdvyr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/galvhwngc.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gmlmumhcz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/guocbmycb.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gqllabslp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjxbyeofm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gsnrlrcpy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gqahcxegk.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gdrgwzzcp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gqxpvjfuw.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gqxihdlks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gotzozzdb.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gzuseitzv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gczskwhra.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gjqfdrktm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/geespnzth.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gnqtlqcjw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gpadakldi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gtzabpooz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gzhdzwgqh.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gyvrnbjpa.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmrduzkyf.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/guwixrdxx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvtqiryah.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gzelypvqm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gruexwwlj.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gtlxbpypb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gdhifgitd.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gwjinmhlb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/giryxcifw.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/griunbhps.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gkhomirqw.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtqkdyawa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gbxbmclca.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gmxkgikyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gqljnnmph.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gnfuyarkc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gnrjdrctt.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gkenbdfxy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gniwmdflv.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjgylve.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/guekhgfnl.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gxtutmmbo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guhudivkq.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gsawxrgfi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzbcskmil.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gdvvkoauh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gceolmujb.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gebyurnxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjnreclpo.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gbfwphrgy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gmwvwpgha.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/ggpwnlorm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gmcuasrvk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gpqeuqbis.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ggwjrhgvt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gztwrfexk.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/ggndsggpu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gjxggryro.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gloatjutn.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gzmccmwjd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gbsfytvil.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gsodcdwtg.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gvxngnjxz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gjhfwxiuh.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gdyjctioy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gifqvgdpd.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gxmturvvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gzfybrmrs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/ghyyariab.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gmhtqibsg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gbnwcihie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gmmemajdm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ghwfyochm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gxoyzkotx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gglqwvnch.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gxehzvjeh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gdbpryaag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gnvcqxywn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/grxnyrgcw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/ggvfdfvjc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gwljcylwo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gqzafhkdf.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gfldmwxmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfidohuko.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gucfpwskb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/grndfxuch.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gnbypsnjr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/ggknqdvwg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gvalonfxw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gdhgnrppf.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/garzxwpnz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gsstdzouq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/goiujlscv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gphshmgen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gduufdhqc.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gigiffloa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gayojsbrl.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gtsaiakmq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gtazripdf.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gkioivecd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwohyxezd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gemjffgek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/geeefhetg.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gogsjnorx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gmradgpvz.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gkjcxlanj.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gxzbuovkm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gykziqzjg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gellqmgqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/geoifhept.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gziqtoeqf.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gvbbhzsto.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gbajywzeb.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gyhharfnl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gagqqaepb.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gsnbxzwdw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/giqsosuff.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gwcpqlizk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gbcqqgugw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzvopcudx.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gfiquvitq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqresabpx.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gynwuutfz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gozlqarim.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gbwnbxrtb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gvwtoakgj.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gjqapimil.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gswocnvtm.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gdypqruml.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/goxechlcg.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gxwgwusum.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gmogqxrhc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/giioikrsp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gyfaxcuol.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gcppjxnpe.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gfcdiifci.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gmykvbjua.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/ghiveuett.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gxbzooqfb.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ggojsrhya.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/guxtiqokw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/goeajwzpi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/glksbhtsf.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gziydqhyb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqpvgsqgu.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gmlnzyiwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/golcfhexq.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gchmqpfut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gqxxxtzyj.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggfmzeojw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtynsprea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gbwczkvqu.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gjuwekayp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gymthiekq.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gzesozjpv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gjmeykaye.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gonyiuhkt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gvbwbppow.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grpksnnvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gjvmatmps.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gizxmzbwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghsgerive.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gowzxuenm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjtebev.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gaibontnr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwwxxsmmw.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmpvihmin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glvyblnhq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gznxyrddc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqmiuqurj.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/glphuqpoa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gbmdpovwe.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gklmmkmam.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gwqampsrz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gxtxcwqzu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gditybsuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gdngebzdy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gzbefqisy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gurquajqa.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/ghokuonly.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gjbyijgux.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gbzdcezxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gmcvjtmvf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkbxzwfmd.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/guysenmke.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbuqenvna.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/guucliuln.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gnbdlxyxz.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gqjxsdkfd.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gqtpfxvqq.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gfumemwom.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/grakmclye.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gfaioyjjr.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gtcvkugao.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gerazlkcp.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gqfnbmzrq.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gcepikrjw.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gfopktdmu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ggeqgchqt.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggyzlzifs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gzricduxc.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/glomeqiwt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gieehsybg.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghesfeben.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gikzdrgtu.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gzkuogenu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gnlyzryee.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/ghjlnmovi.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gmsefawqq.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gwnssektr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmyyxflxf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/glhpsaisa.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gkoxnwnmf.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/ggrvlhuos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gtgmqejqr.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gywpbobbc.sHtML


<!-- 参考信息 -->