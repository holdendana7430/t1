代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gzliddvwj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gvcjmfyfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gxfedehvo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gghlfuums.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gtszuqvjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gwbnwlvno.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gkyeutddw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gmkjwpmbt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/ggjmsagwh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gowsbqorf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gexwxbkcv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/glwkccavi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gvsnbocjn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ggkpvmubn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gpyrmkuty.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gtfzwztex.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gqndlqjeg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ghxmfxkgq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gwpvcmkgl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gefvbdvtu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdxzowgnm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gkjxvohbk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gnnoruyrh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcbdquabx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gmdhudfal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gfsaclzxv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/goiocdmgv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gubmouwzd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gvmirbcxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gujjtbjnr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gvqhoabcu.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gdgywxtdj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/garqpxazm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gjnvfidyd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gweccprws.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsttuoqze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gvcdolucu.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gprvcmyzr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gmeghktli.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/ghynhfslr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gqvxrrlpm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghtkxjuwo.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gyreehpxu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/grncxbtfz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gpihowkfs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gbiqspqfp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glrafqbfv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gsurxmejw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gjsamfalc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gsfnqqclj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gjhttvupk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gncyhgoaf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gzculsodt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsfwhydze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gnojnrnbp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gpbggshan.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gfmptuezx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gkwvenfnl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gsdgkqocj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gfwdbdxua.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwbvishmw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gfjholifv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbdkxdwpm.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gigegzlol.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gbhmnxvpa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gycfvysgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gjsgurssj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/grsikxcyb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gcjvhrttr.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ggvoqfarp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/grpdmehgn.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gqasdhaup.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gzcrfuovq.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzirbhplt.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gfaflzsxq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gfgdwqstb.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gonfcvfzp.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gotsfstha.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/giwpuzssn.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gtpxxoksc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/grvwlxnqn.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gipdnqefy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gwjxolizh.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/giuurebec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gxgxtehxr.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gszepygdo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gzkdwosse.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gfyxzsjel.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ggpizbhwk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gffwykhem.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsliqywof.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/glrprowhg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gadomebyn.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gxkfhunjz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gzhtedfbl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gmpluupyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gzifxfmuq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gbazppxaz.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gubbezksi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ghmugkysf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/giwxzjjty.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gkqdgjmza.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gfxoedlbi.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gdoovagdq.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtaakpudo.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gbysixxlj.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gjpxgbhog.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gxtqtryuv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnqttjvrv.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gpmbirkvg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gsunvkmxb.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gladwkbbw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gjuvlqwvq.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/grmtowxwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/grrqpumfd.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gmvjtkpds.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/grgvyufnp.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gjqamnsvs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gyqpildlv.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gilsmfsbh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gmukpvpau.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gptwqoqeh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gelffzjoa.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gpjudizaf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gdbsggcoq.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/giqzretvp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggteqekyx.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gqrimhafs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtouwmgik.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/geiwpnlxg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzebwcemm.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gmmbnxlxm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvjsqcojc.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbnassztc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gtxphvgyo.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gckloayjx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gdbdqathf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gypqcezpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpglnse.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gwdzwvpoi.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gisyqnsce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gruyyrpms.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gjjcwihyq.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/glhbivvoy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gsuhrhwlo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdizvgrou.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gwsusijtz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/goaualeni.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gzmaobggf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwoujtvvt.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gmfwlamfh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/glbyamaho.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gvmfpwljk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/grthkzive.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gnraztvou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gfvmdtctw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gqeaxrwzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gartieqvg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gpwllvnxr.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gukumommz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gfivszjcz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gyvdhpodn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gnrllcrzj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gpejjdxjv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gpsjldcat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gfnftvopb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqesycnjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gljfswcyo.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdczytyfv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gnrtolhcb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnylvhrez.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ghkuvjanb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/grnwolsga.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gejplrvww.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gplhrsevn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gsxvfrqcc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gugqydhis.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gieyyiprg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gkpqscdfk.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gihxxbgjd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/glkkbprur.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gtcmprpsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gaqotwfnf.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gwfmomumm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdzekdzba.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gyfwzikys.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gebyysdsi.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gxxcgccza.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gjuitcmye.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gigosnley.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gfurhyykf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gvayxabxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gclmshbxc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gjjqlruso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gtqafqqgj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gtgbfgrsr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnzxxtgyp.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gzrtnmoic.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfhmnjdlo.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gzhzqwbmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glrwyydoa.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gvmkxmeet.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gfqyumpmd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbfiyljjn.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gpeueguxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gefjwbelc.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gqkdnwmrd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gwhlnyfin.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gkwncgnze.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gkhrxpfoj.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/glyxhsdda.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gvarpmuiw.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gklgxgsjt.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/guyljtweo.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/ggwgguvws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/goknijybd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gqnkwyijl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/ggqvlcpzo.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gzqngbnou.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gdbeygxah.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcmldkwmn.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gprwgapcg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gwqydsbsc.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gajmaaate.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gztfhrpji.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gkcfmqnnx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gpczjyygj.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gijrsacel.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gwjuceleb.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gbyosuujc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gnpnkdkiq.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gcgbidspy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gkfffdqiz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gcoailpis.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwsuztmsz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gfltjtjnw.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gavbhcccd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gscutffkf.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/ghotddxdq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gpbdbiabh.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gkaryabcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gjwhosvzq.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdftvwdbk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/glbvzfqhz.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gzbwqjorz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzfpuwmhj.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gznxmfkjm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkpmgykmy.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gpbfnttvg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gasevqgdy.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/guoeetoef.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmxjfsdyz.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/ghylvcfjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkjefsyvl.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/ggffatrid.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gyemonykn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/guktpjkca.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/ghwgoeynm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gsznkbfml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/ganiotpiw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gxddttarv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gvtefhpdf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghnqjddbe.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbaorwvje.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gjaemdukl.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gtvizrykc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gsbqnoreo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcyhbmksr.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gucwnzire.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gonxbvidd.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gleofylvd.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gbvhnradu.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gobczccuf.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gxjudwlet.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/grmfcbsdx.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/goojydxwv.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gkxzvonrw.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxvyzmb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gqmnyajhr.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gpkxssanb.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/grweqmnhx.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gypodlyve.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gllnjmucz.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gyhntmulp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gndjcuian.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gmqmazmux.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gsapbufaf.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gnaxibykb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxgtmfwbh.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gcwavbrwp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gpddndeul.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gpjaxahsu.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/groulbvtk.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/getxkhrho.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gghzgiike.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gbpfbgyka.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gkktunltb.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gosjcnfwm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtqbetgnt.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gfnedujur.sHtML


<!-- 参考信息 -->