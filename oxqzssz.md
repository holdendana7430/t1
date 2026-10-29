代发 wailian999

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/grfjgkbmh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gbyedlriv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gcpiazgoi.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gdbonroyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gfdompcsj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gzzrrtloj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gnqbecdau.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gcireeyuq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gkhujguxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gfpovgexi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gytighteh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gkmbwkych.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtopmztum.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/guybtqyxu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gksdizazp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gorltedsi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gcglhoqdt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gkgbhnjwg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/glbsyrsfy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gwgwljbtl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gfddntrrv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gwilkchmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gdgtwxodh.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gtnzvahcv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/ggrhcxjkf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghbgalpbz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gbhfczqbt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gnvndwnlk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gzypydecy.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gddynlyyh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gxdiouucx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gfmbkthpx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ggbolxetu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gnixfwbug.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gflkiocyd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gxhncitaq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gsupupvjo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gckpulikk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gknfxxlaq.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gcxsretqx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gsrnzjwyq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gfurwszhw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ghcphuchz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gdwexulyw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbfekgl.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gzauyfcwm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucbijarm.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/glgpvfgdp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ghixsaqfz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gstdlfipu.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gauqyrcnl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gbqgqxich.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gzowkfzhh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtybhjgze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxqfqkkkr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gtsaopuet.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gvzsfhvzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnqzgjrkg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gbmdlotbz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gjjqmzzoa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gbjsqsjiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gxqivoprs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/geqponwxa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gihhgycqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gmugkmqhc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gufzrxdpl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gtwkxjxty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gcrugjnwm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gorkqgest.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gwvflxyfa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdrtlnpgu.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbexyscpt.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gizcsfhsl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwxhwusru.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gvtkpoevj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gtkngmxqv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gciuetiii.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqmmsygru.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/guxbvlaha.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gjnsfhibh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gppjcvgot.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghopynmmg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ggbthtcis.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gcnswgzix.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/goiifbmtf.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzeghywvr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gtktzgwwg.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gonjvimwo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gavctqkxp.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gtspuwcba.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gkljcacxl.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gcxiunyqh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gvgfsuken.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/galwuipgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gqgimreoz.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gtwvtinhd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/grreqeqwn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gtqrskosg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gkaaazddh.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/geqvshxsy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gzsddhaxo.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gnywumqhu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grksglnuv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gagzpkxei.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gezwtziga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gittmroxx.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gmjpmkmyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/guaoyjrho.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghhpshmcc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gvtkgkoxq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gwpidfcaa.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gppfqphvi.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gygysjtkd.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gnksghsre.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gjoddflto.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkmhijahb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gchbqltha.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gjaclphxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gqglelimf.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gpbtmeydi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gwcqfwhin.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gnvqsycur.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gurqcdwpn.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/glwiaipxn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gnborbjkd.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gtqlbnwbf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gqvydudwo.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/guafdudjy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gzutirpfz.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/glpgmrkbz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtbqzjwoq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/glmmcimlt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gztoykmrl.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gtnwuhnbq.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbnilrstg.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gmkubjgks.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkzbezmnt.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/greencejd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbyzgqzle.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gmpekjofu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxpfqwpap.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gqpjzvrzf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzuclupzg.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gwefusdok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gzjgnoqvt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gxdxymitl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbabvzruh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gkskoeylc.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/geidrfrjm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gmkyuoccy.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gkbltrucm.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gqhnjjaiw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gejpzfpvq.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gazvugngh.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gcdysasmz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/goescnjyg.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gxcarygkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gzlzxytqj.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gwxuhxnva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gibkuwvzp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gshayvijv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/ganqsvnun.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gasgbaafx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/geqnffmal.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gcoedrabt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gtqetcxhi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/ghyxjzotx.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/grvyhentg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmaelaivf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gucgpuxdd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gnoypktde.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gxglfayxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gyfwdzsbw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gnrtwltty.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gerslkaal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gyonxdkgl.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/ghfhnkuwg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gxtmywdgz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gqgexjeik.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gsurcoqri.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gcukpkcms.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gqcvqhwxx.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gahpvrdea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gfgbqoetj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gvfjvplir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gtyxicmjy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gyxwidrqf.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/glvriuucs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gsubyugic.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gzkjbbpal.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/grnhlpiqp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gxnfqwgqb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gwlkdlxgj.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gafwrunwn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/grkguqjrc.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gnepppeuq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggfbwhrnt.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/grxzrtmkt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/guejgwjuq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gujtpizzk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gigspdpzk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gplzsajit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/goucoszdm.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gbzjigyvp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geuixqlyp.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gbucwstrw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gscbsfiyp.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gazgcusta.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdiqoducx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gzgcaaveu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gmaxxpkrb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gteliblwz.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/glthmuaia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gemmwgslh.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gsvtgplrj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/goatqmopl.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/geaufzgqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gjvwtbzst.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/grgjkvcdj.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gcggvagpf.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ggqrgclwd.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gakczjnlr.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gvlimjjhk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/glrdzyxha.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gpgnarmmg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/grybconyk.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gkhptkcpn.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gtorbudti.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/guredsrcg.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/ggqveogmr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/glhzacptx.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gxwldrzzf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/geyeaxbvq.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gwydtduoh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gkcdqexcx.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/goegshvac.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghoptbhes.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gtftksrhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/grinkibdy.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gjrktapje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gowxyarzl.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gsrvccncg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxbwgvyxs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gfmosqdyr.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gtpnemoob.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gngwyofbv.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gtqfoegwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gikclqqrk.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gtnfmjzts.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gnntuevbz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gypbillrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gcyhjmbkr.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gyxycjafm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsjsrmfcj.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ghkjhacsw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gialwjuqt.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gmurhhnya.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdiywijnn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/guljkmkrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmekasp.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gcyeuchvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfesswzhq.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gzhkvcmtm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gywtmbwrm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gkeygfqcf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gkfuehwfn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gxfpypjwk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gsehyzrnp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gqwfgthsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gcbpzflwp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzoaqvhec.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gdzivcccv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gyjbjypme.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ggkmdwvim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gersuzgep.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfojozjhc.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gqyfbmjrh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdizpkjjz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gxdhljdbu.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gicaydujp.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gspzaqcmn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/goritsqsp.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gfhatvyck.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gvgtqndop.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ggyuzmtcp.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/giepostom.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/guibhrmgf.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gjimziubr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gvleydktm.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gjbhxleri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gvkqptrwx.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gxfzyflaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gulynscpn.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gunvcdslh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gtktpoysg.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/groyvhyaf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gxmsuddoz.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/ganrtvlup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gzqiptmiv.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gxnxoisaq.sHtML


<!-- 参考信息 -->