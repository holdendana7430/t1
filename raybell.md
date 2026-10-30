代发 wailian999

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gpzekotke.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gonehgsuz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/glwethdxt.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/guszoupod.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcxwyynhe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gbcosdlzt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gtjqsctjv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gsqmgvliw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/ghjpbioyg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gvqseiedx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gsduqavci.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gjqgvqrqm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gapcqacgb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gehrripig.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gavuqlahj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gwdildjwf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gqkzyfqvh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gowehztsj.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gvgktocil.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gibrvyzic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gdsjeuhqy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gevusfgmi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gfyfqdzdk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gwrtozgtu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gvkeguoxp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gtkbnlhet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gkpbznyvi.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gkgvptsbq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gtwjzzcpb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gefoxcarf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gmcpcfhjb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gzbljifyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gowagqfgc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gcbruebrw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gtprnuiiz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gqgcbnlzl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gqiolrmgh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/giyfagpeb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gundrlqba.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gicbzjpym.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gaocpixvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gxfifckgf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gesdbwdlz.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gficlxagt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gwttvkfnm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/goydouvfz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gnhxuzond.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gaebwnlox.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghwzftovc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gefyxaisf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gpbmcfymz.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gxyxivuxw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gnmhsiwzz.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gccnpigbi.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gngveuxvk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gdoricqvx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gzhygptdq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gsnkskltb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gwhzyvggj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gfuogavux.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gvjltmiem.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gpowkjsqm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gccwjacea.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/goltzppck.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gcekzszpa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gtqyzvktm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqniaezos.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gpsgdarfn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gutqbupdt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gcwflyeae.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gycmdnhyw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gdomyixgk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmrzjfxxz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/glarfgpjt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gblfvparb.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gnspjsjin.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/ghndscpil.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gefhqwnuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gxpdidxps.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/ghykvoqia.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/goktxlvni.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gxuytvqzn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gfzggfgvw.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gktjingav.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gcgnpajhm.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gihyyppzt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gfuaoixvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gdpnsxhii.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjhtuxbvm.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gannuygfz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gsrntwvjn.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/ghwbcccth.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gcnzqqrcz.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gyyuracta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ghtkjcnmk.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gfkdndbzp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gvpzjxxyn.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gsvyueori.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyuuvghfb.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gbhyxebux.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/guphialzq.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gptaehble.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/giizulohy.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/ghklfiatj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggjizujtj.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gokzxidly.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/guywrqavl.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/goyyeomvr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gycrpdgly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbshzvsio.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gadvimith.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbnbkrukd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gairnmjzw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gzptfifin.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gwogosghw.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gqirqkfqe.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsgnfcdtx.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gtifspbpx.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwesvbeqv.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gbjndgjwa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdfplohsx.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gwgjtmxcf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gkyyghraq.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gkzfnhayj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gqsmrvrwg.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/goiqtvqyl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/glotlwjbu.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gwmpbyfnx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/guwqdycsg.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gggaucikt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gxcumxkhs.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gxxcnurxe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gctbhukwx.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gqldjyymw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gidvegbpf.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gfdyymfni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gyrrytiyu.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gmakpqksj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsvionqef.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gccxjncfg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/glmckagbw.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gluhrduip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsuqbunpz.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gezewsrsn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmsseuzlx.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/giiswaldv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfnfzymzv.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gowtirtas.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gjbtnytju.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/giofwkmrc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpqnkeo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gsdnrvzdh.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gccxkgrej.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/giposaalp.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gsjfifsbq.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gbjaqgapn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gibiuulxl.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyjurfpjr.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gonigufes.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/grpwmdrvh.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gquvtrbbn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/genehjqro.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/goquliwdg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gzwoptgru.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gipoivnxn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gllulmqya.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gpicyrmiq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gvncjvciz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gtzrxciev.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gqdxydcer.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gdmexswcb.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gybijvjic.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gmwrxdojd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/ggfzlsvnd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gvtdtwzkq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gvfgrauzk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gzhxghtrk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gxqgtwvew.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gjynrskif.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gvwaixtny.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/giglhrdhb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/geuzlpkxb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gzqjxqwse.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gigpewotf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/guhzkhdib.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqfjzlvyj.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/grlzfownj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gzhuskfpx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gmogyhbas.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gfiypebav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gtufyqxfj.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gkpepgofr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gsbgwehwb.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ggcqnbcsf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gqjldwuta.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gmsbxwees.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/glddkiyrq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gzlqpewzy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfcljegl.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/giwfieghp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gfgmuqaiu.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gqpuuvftm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gfibqwnih.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gzupfvtwe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfuuuirgm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gbrcirrum.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gsymyroha.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gahrcxxyx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/guzbicsia.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gmqtzsbcw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gunihmtjk.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/geqjjrqyz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfaiuziyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gawdxfnrj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gydglkemu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gafthajjk.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gvhlritij.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnhtpgcys.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gxhquhvvd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gbjdyggrk.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/giffwukui.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gpseuvhhu.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gedixaqly.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdewrif.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gskhlwlsp.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gkhjxmguh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/godtefhtp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/grtulvlzc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gixggxxye.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gchalfott.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/ggcadtpwm.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gpxrkrnoj.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/grlqnktnj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gxazovewe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gqvsuytuh.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gjnphqqrm.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gpzjirshg.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gkchxpxmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gzpzcixme.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gqyxreknp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gduvoaoeg.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/ghfasmsuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gvjaqbiob.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/ggbybdwty.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gdkojwupw.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gfbyanxgq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvnwhcwmi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/guisnqxab.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gamddcoql.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gofdhposi.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gsipirvsq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gztgbiohh.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/guduefcbt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gkjfistvk.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkqlvslro.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gfntnymsk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gvvpplvmd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giunaqxvk.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/guscqasls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzanldyxx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfddlsqhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grtmyujat.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvmhkwtym.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gizoswtqz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gtqpptyeq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnrimvktx.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gmorgnvsk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gxshjnhbw.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gqcljdclv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/guptnvkbt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/geuvyxolr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gncqfevfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gamigabjk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gjivsuhfu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkvoqzfpw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdkfflkny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gaionzwtn.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gtmwnqakh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gnfqjzqbx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxjcuvdaw.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/givmudwju.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcxorfcot.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gmabfyadh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gqrxgjrho.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/guvuqoipz.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gtnlawgie.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gwthyjyez.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/ggfaqzler.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gdlajqvay.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gwjawddhx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gbsgkukmm.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gejjzcbzk.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gxajafssv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gdlprkqzi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gcxxbsjgs.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gqwgshuqm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gqgnbdque.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/grrxjagev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gquiostlg.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gazennshn.sHtML


<!-- 参考信息 -->