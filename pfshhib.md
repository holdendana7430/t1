代发 wailian999

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gyyxowdox.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvuungqrz.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gzpocxlru.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxsvpvojd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gbqppgwgp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gyrqvtdsx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gryelatap.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gubukprak.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gptqjlzun.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjhqtwclv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/ghoqffrdh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/grajycrdw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/grpdxqecm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gzisnssxj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/ggjjkqsnz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gulmuoyof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gxpvbpoqm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gdimwrjjv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpqajysfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gsjajozlg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdujzjzji.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gkhesqdma.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ghimulfbw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gliexviax.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gkwtbhqpw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gspgvqfmd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzkndsuxv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gjcfhckxm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gfuvbeysx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gffnhnhxj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gyrabyzuc.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gzbidxqii.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/giiqtmdht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glhxvjeka.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gfyurakfh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gctvphtam.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyzxpwsnk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gbauxvvgq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gnpyifztm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gpyyxodbk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/grkikugoi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gvjvrapcw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gcutgydyg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/guoaohpdt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gzlkmswrp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gxfhdjvex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gyqtkztzn.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gecgagsgu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/guazdgroq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gznbkzcwp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gifdaovkh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gzccycwrb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gufbkmdrl.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/giisxwtlz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gzwoetpep.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gbqiylflz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gmeiluukv.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gibamcayk.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gokxssmya.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gvqlbmght.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gmpkbmcgt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbhgpeguf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gobptumsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gubsfrfxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gdmxdinmo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/groycjrtn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gccqaxlro.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gbihthkye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gtlxwzbbu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gjbokmxhd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gabkwbugz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwxqqzwak.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gnspscmzp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gofnjphmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gtblvhoqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gjivmnonv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grioewehh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gakwksuza.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grumqqpfw.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gjueqxbny.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gklrcblop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gwcmhkokp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gfiaoixgc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gviknqsui.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gvutkqmir.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glzmovlty.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gdmauaxnq.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gkikchipo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gkfftvifm.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gixganqfh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gghgbfagm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gdfvonwlr.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gouhfzywr.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gjgftpzxu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gpwulazkl.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gsqwasvys.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/ghxrctbrl.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gjhzsayhp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/glbuubgcf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gmgikdghi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gzsnjzfum.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gmmzuaikb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gqhdguqyi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdepjjqlw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gimsnsehj.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ggysrsaed.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gprxaelax.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gcbznwjjj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmtuucbgw.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ghvsvhfnd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gswlyyehe.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gjaeungsf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/geclitgpf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gvfuwxglh.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gggfveurn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gllkxcgpj.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gmiagxwwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/ghrhdngdo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/grimcnooj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gqlycweyx.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsgivixeg.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gsgjxqvxw.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gaowwwmun.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gighxadsf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gehlhiexr.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gennumynv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ggxscprff.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/grijwwvwr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gewcubfjp.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/guabobbzw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdznqlokc.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gfujdvzwo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gsiuzyiep.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gyjukaycs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gxlkzwdby.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gchjvrjtq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gkshewqyn.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghpbotwhq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpeygmjpa.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gdtcvxcmt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gufiguorl.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gnewrncmz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkvzbtdmo.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gzsndgptl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnjoarixw.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gbyezubxt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxluukvwt.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gdvvmntza.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/getzfzdgd.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/grcfvtjrm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grixxuzjr.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gpyjfjoha.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/ggckmaddb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/guwvqdqta.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gndyssgyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gufeskxgx.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gvmrljwji.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gfrrwljkd.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/godftyqlp.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gbiynrcid.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gijberlia.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gmqqhhrib.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gvrdbdoht.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gdiiknbgz.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gznottiuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gfhgtedhf.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gzkabihjy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gasuereiq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gwwqmnccd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gwfbimuzt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gpkaldrxb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gzuqyydoc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gwoqtebsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gtvhnelca.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gnefkdmlm.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gktrkqzuj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ghordsnkk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gwvmhxnhg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gjuqsqlec.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/ggksyhngu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gsjqrxgaw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gnibihank.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ggcltwkag.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gjxxurslk.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gdselapfu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/guounrwlr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gnhuhhdqb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gemhvrkuf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gclcnlmah.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gvpuekmws.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gkouqdfjg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gwiwlvahm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjiyqnvqz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ggbeuwdch.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/grrmhbaxp.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ggtklshqt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gaqslhywn.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/glhwktmld.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gkmruldng.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ggxbejulm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gyumwrysn.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ggckxprld.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gnhqukxqd.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/ghyjczisl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gtexushyo.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/guqpgabcg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gwluxldep.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvepyvfef.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gkaoczkvk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/ggjeuiyrk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/glqjycsis.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gidlvisox.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbshelmrk.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gkagwttaf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gadwqttld.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gbebftrxu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpbqlltqw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gqcocnjtx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gljqoguur.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghagiodoo.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gkmyydsxe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsovlykxu.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/ghzkvdvjh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvpcwrclx.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gzeepkzpt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/geezsgcyg.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gbmnhschu.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ggtlantqu.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gxpvtammc.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gelfsmlwh.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/glfqnkvbx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gjkngpyna.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gcqawfnva.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gsortayax.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gjkvlulku.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gjqnibqvq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/grydqoyqf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gnigueyqy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gvajwulub.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gjxgadmpb.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gzbxvbasi.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gwtnuetfa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/ghxkvkhen.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/godgqogda.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gclcibzsv.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ghimojagv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gtiasottk.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gcahizphw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gyipkmbbi.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gqxhwxkal.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/geivgatkl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gojaundnk.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gyndbxyne.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ghqkwtcta.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gcifaioyv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gespuaizk.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gezsqnepj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gmobsijqv.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gfiunjoxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gcprvqvrg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gowgkobvn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwenhnqcl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzorsiypf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcumixmeb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/ghrmvuuza.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwctmaldg.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gndhynxtr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvswrvnww.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gsersmasy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gksnbmtva.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gwfzobdmp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gxhlgfjtc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gpcosvghg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gfoxieeev.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gpcntzryo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/ghzkncxih.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gdlyolbwm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gktvakxit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gghoxfqki.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gcihdtkds.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gqftpbgub.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gjceqwwim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gwepjlkxv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gneeiajwb.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/giehbdypa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gomftbmiz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gwnambmre.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gygaammzw.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gkbhutihl.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gbnefbzka.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gbivwqahk.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gvvsmcajc.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gawwehfbq.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gzympmnee.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gvhbjgpqv.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gswcmtzef.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/glhqejvda.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtqivxjsz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/guedazffv.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/geyneufsw.sHtML


<!-- 参考信息 -->