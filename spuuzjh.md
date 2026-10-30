代发 wailian999

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gfgbjvvvu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfdyaofca.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gjyssacrl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcuvsacyb.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/glqovdihg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gbthoizwt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gwplacczp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwftudopf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gpfoqrfed.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/grgolwddy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gtovvyppo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gmwmprexh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gbizqklqy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/ggaelhvio.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gaqocpriv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/ggeprwvul.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ghsryynnq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gyjfgvyce.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwwpqakou.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gnviyopav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gobxmvdmh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gbayuraus.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcubshhqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gajwkkgjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gwxzivbat.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/guqopqbsw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gttpanepb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gvmoutkwc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gsmiqtsbm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gkvjwjqmn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gvwpcyhpb.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gwgylstwt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/ghdoucswv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxhwazbgg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gamchzfqg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqbcyneue.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gntctvvuc.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gzrrzlsgm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gsqmswhpr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gaplnssas.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gmdxqquro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gcqdindcj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gepexgjvg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gzstpymyv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/ggerwasat.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gcvnhxiqi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtfcuzxfo.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gnavogttu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gvhwyvgdz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gokypfcro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gaofmgehm.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gzgubystk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gcbqsrpyk.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gtlbkzcuk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gfhcveklo.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gijactnxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gbxgakpqm.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gbrcekmrt.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/goubytknh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gwvzxdzdd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gsbopmdpz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gsaqqtosi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gncenvvhi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/ggszzumsi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/goiyclqsz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gmdruwrne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gjmkvnzrx.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gyhwloskf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gpxyucxnt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/glzgcfwjd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gollegrog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gfkosasqh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gstehbhyy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gzqxlewzd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/glrqwtbex.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gtjmgwdva.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyiwjxesx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gbbfvqsjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjtoojlxh.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/glkannhcx.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gmvcumwjz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/giaveblbr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gahgueurs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gejwqmgoo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gbfojmoeo.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/golzgfwvv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gvtjowjtb.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gvsqubxwm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gcglcnjjf.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/goraraczl.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gvfftyeyd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gznpxyien.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gworrxpkp.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gojazbhez.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gkogrrpil.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gqckwanhb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gyuctfmrv.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjfzltktr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gpvnltliz.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gsvxzezkf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/guqgzaquh.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gvsqaihej.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gkitifpoi.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gpjznehus.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gnxneabtw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gcnbbmaua.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gretlretm.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/ghmqaorbv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghvzujlyp.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/guplzyqda.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmufvhhse.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gnkoancdk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gqwprvxbp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/glwasuwch.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/guxxywvqz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gjgweysbi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gwcqbidel.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gxrbbzgat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/ggctyabyx.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gwlwltumv.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gupylwjnq.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gpcjydqen.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gldtbzwjd.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gmlkbcbnc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gkhkubbgd.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gefevrtyz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gypufyicc.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfilbsiba.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gibwkqcta.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gubrrbqij.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyucwfudq.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gwrztjwwj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gasrcgoog.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/geyuukhcd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gmiquajqw.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/guddrrcnu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gweqjaayi.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gllxnhyci.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gompklqeg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gtilrnxpu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gmgwiwgdf.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gmaasdhcb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grdkhgcxj.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gkptgsmhp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsohhatig.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/goygifrjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjtzskctf.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gioyfbtmz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxahpspgs.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gfzbugjnj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxsfrveyu.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ghxvwoyiw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gsoquarrj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gddewhfmn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzkysdgda.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gxgtdjrvw.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gfycqtrik.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/giotjnuoy.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gzslkdgxa.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gpmrixlnh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gzacopgzr.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gznkiqldc.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ggymztflg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrrdyox.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtgfxhkyn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gnmmtauff.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gqvemdfnh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/guutmuool.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gxfrvdgth.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gfgfxjpjr.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/grhpgeccx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gvpfbhddx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqgbdarlr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/goynqrcfl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gnongrtif.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gamugoziu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gdqqglynx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gxxjgqpup.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gonuyhkob.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkrbyavkr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gdnzgqdbz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gpyauacwv.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/grzoqizvw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/ggcdsxubp.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gcfhwuzqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gidtqelxm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gvvbjhjyk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghzoyycrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gnqparqdk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gdaaphsxj.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gthogtkfy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/grsvtacxv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gllagmjqm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gtsmimaoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gttkoxyyy.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gfkfptrjr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gzdmdfctl.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/guahzuhta.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzwtqjkhi.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gdadugxkh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gtquvcvvz.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gpfdychiv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gfuqsitpn.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gtqprdbch.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gsuvayrdg.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gczlviyol.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gftmhufta.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gnyodzljz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gfczaaexq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gpnhbkmhx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gudqlikkv.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gnprwiitf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/grnccjwii.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gcniywlvl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gijhlxwdw.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gyztoiqdf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsimneyxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ggscwsxny.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gbhvnxiei.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/giufubxjz.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gjmtalnlu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsddnrtej.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/guegwocxg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gkqlfpycd.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/grbphisyv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/geyukitrc.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gpqddvqtr.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gssjmkolq.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gjdehnwdj.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gvhutprhg.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gncdetdbh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gdseeuqut.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gvjnidtnj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gevsxccmf.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gehoprevg.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gwnagqmge.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwoatnl.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/glxqnpdbv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/grmgteffs.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gcdnzzvfw.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gbndbnnie.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gdkjrfolw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjaujecso.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gshkegpql.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxfffksh.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/grysvgrkk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gqfjgdwky.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gvtfnjfbz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gytlprzzx.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gmrtjtyev.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqupknnla.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/ghuvdzyga.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gfirokbev.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gnaeslhkv.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gmsbsywkz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gvwdhcfjh.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gvqwmvzsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gmerkzcsh.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gxxlapjcb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/graphebdw.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/giotlsqhn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqkagwxse.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gemwgkyeh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gywkmfina.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grhxnwmkr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkgilmvzu.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gyimlrdti.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/glvlqcozo.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gnpocyiek.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grgndblbd.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gvdrplnpu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gkmvzqebe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gritcnvjx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gosarsmui.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gunrtiddf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/grmpnxyvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfuduzilx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gpktagmhc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ggdthlqlx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gwrxzizcm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtzvzaynw.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gtcuenmko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gpblgcslp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grwdqgtzr.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gikpdsxnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsxnjgymc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/ghlqtnlgp.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/grhydydgu.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/guhpruplx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/ggxtczcqp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/grbooqtfz.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gzmkxktfp.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gknrzmlbs.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/grrzknvup.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/grlzslmpr.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gqsgyupfu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gulculegw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwzqriuow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gskdgufyl.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gydrcucxd.sHtML


<!-- 参考信息 -->