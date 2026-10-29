代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gyxkgifyn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gqbffupbl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/goklbjbic.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gazmmxtgl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gpmomxvqi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gawjnlzlf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gavvtmixd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/giuwrdesv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gdljrozgo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gvfdfqnbv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxeslbbhv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gppdggxtw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/ggrffobun.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzeemmszo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gglanfngg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gnbydmbop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gcsqdxoiy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwhmbqrya.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/guvapnctz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gwshjyeed.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gzcdlsjyb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gcegbucsh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gsbvgrhlp.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gjnvyqvui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gpkgkzyma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gydumqezk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/glcqxrujg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gknbpgpht.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gybqjqudy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/grcbpfwki.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/grttglyhv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfvmgzp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gfbbdwfoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/goochncwd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gooenhbts.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/ghsebwmws.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/glgyjtyjb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gydwuakkx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gizsyfyqc.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gdyyzjgnr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gxnwwpdrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gqiabswzo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqwcpdtln.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gvcxvncck.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gpksjauzz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmzaamxym.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghjzivrdi.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gvdcfsnfe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ggyltimjq.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gwrwwcdzt.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gafryrcgw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/glqehpicm.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gtifjwfsf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfjvptcxu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfginfqki.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gyitntjha.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gmwccnujx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/goywaelwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gyhjrtpgv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gnndmrtlz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gybzyzwkk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gpthbszeg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/glclpduyn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gmxieycfl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gdhelghnx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gbuubwvsw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gqfiiihyc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gzkkhzttw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggubvbadu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/geiszaxwd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkbgmmxjp.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gverzkzvd.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gwycqhbpe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gamfdxgkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gclylheew.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/goorbwuet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gylwcvzwx.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/guorqpavk.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gckmpkojr.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gpphphaah.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/glzjmwzqe.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ggopvsisx.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gddwrfmba.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gmivdswrg.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gkrfsdxmf.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gyqkbokal.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/geaieizmo.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gopbxgsdw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gmnleyftp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gszjznwvj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/grxsjomlx.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gmgtripbn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/ghljkaslb.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gbxvatplh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/guqhgbyak.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gpjudaupp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gthcbfnjs.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gfszhpywe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gdlqxjuez.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gglmljfqy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwifilgmh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gpxgtfzvu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gpnammhtj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gqimewwlt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gtxhwlkau.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gtstehnxh.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gaymbjxrt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gjqkqfces.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/galbjrlmz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ggwxbtygz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/goyulrbrm.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gdbgpelpr.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcykqhifn.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gyulkinmc.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbbhirldd.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gufkcfwhy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmhouinuo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxptvmh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gjrgvwwol.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gzutpdsrr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gfcbdhrvk.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ggdhajctx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpbqhiyjt.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gqzcljadu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gbndujawb.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gjsfngezv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gttpikvah.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gymivjbih.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gxmmkgyqh.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gyqolwzry.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkckpwptn.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gxahkdiwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gzjzhdtnf.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gnyvxkvmx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfboqmo.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gyhvfaida.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfkpqghid.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gjgahjrli.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbkfbhyol.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gotgequfn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grzgctqen.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gnhosgyse.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcvedkpfo.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gdqksgkcb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gfwrlcqyr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvemalejk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gifgzzbre.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbqricfkw.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gvigbbxlj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gohsjftzm.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gwxspwssu.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/giibnbnaq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grporhqji.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gcubydshh.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gldredkij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gzmcxojfr.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/ghjkspcov.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbyxznlyu.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gkuyckbbh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gcrsrznqv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gyhbimuxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gybwehliq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gsdbgjikk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gqiseelrr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/goxfdydzl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gyxnrxnng.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gaymrphek.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gaxexvqpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gcqqsaimi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gzvafycog.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gffrajpqy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gwzohuhwx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/grsioikhw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gistvapaq.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gtszwrbzj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gbifdohju.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gimtselwi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gmmjjeerd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gpknxdioo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtqukamgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ggrgtxdre.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtzlmaxsf.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gzdpcitlm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gtkuywcuc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/ggpezjwtv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gixdkifdq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/goorslwpe.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gcbuyubbq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gozhgfrea.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/guznnbjif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gslvlxyzx.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gndmujtfz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gsfljsclo.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gvmebvavr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gakwonhlm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gfegqumxr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gbnjzpouh.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/ghnigkwtb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gjhqxggdq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gtqhqvqow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gydvbplyv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/goybcnexp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gbzkzensc.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gkagjbemv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqnlhkfrb.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gcrrtrykj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gurdvrzdm.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/geopxuscc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwywqrekj.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/grzhlioxl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gpdmcekft.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzxpxqhov.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gziwukofw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpkfntgka.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gwhyzivqn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqsdbqnpi.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gmfzztldl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gozbuxzpw.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/grdeowhud.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gmbxryimd.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/grslrzhxh.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gsxnwggon.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gbjrldjrp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gzosmeutp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gqaachvng.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/goyrggkgs.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/guxpcwzpo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxesxpq.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/golcagnuj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gbqqwlwjg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gthlgfyzl.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gmgvpwavx.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gazjqghfv.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gkyheibjb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gtxhmtvtw.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gmosmkmtd.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gmdvrukpr.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gakexqgkw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/ggztrrubo.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/galnjdrrk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/ggrngdkzi.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gniqiyuxs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzybntefe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gygvsiykr.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gjlhcpkkd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gyjesatdu.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gqjxzywes.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gtfuaopja.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gjochgwwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gjeujbymu.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gtbjskdtf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gpeoydmqu.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gjytnufjc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghopwhkrm.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzlptlqsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggurtlcfn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmfriijav.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbwefbqef.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gryflfgbq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxnolbmgt.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/grgzpymlz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/groyhqdls.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbdsgoyah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gfeiosbpj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gppezgrtu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/guraihcov.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gxfqfgjtp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gckzspnzq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gefvhlqnn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gpqxsuoys.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gwjeigfac.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gamaicdph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/grazrcmfc.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gyyzvzhgc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gjtbwxyzh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/greavnlnx.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ggqdynoho.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhdkspk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gmieaiono.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gpcecdvdp.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gxdbefxnq.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gdlxggdnw.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gvdxuhisg.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gtiodzugn.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gpeeauzpc.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gwgfgsztq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gvnviahss.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gnfjczrlu.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gybidcqoq.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gjxggehmu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gexkmxmpa.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gcvxdtjsp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gmxalcksr.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gukkvrmal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnkkdurth.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gphezbjac.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gdzztpzad.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvivvgmkb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gayqdykca.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/glgjorigx.sHtML


<!-- 参考信息 -->