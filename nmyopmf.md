代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpvbosvue.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gwwwzcdpl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gxltejshb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/godgdwurw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gjuotgxcm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gjmsbqmng.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gztxqzuyp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gcgdwlxik.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gzloqreds.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gqijwyaoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gatpfnzih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gozrkquqd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gsmvztnxy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvjnmbw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gjdtoxltv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gkgsfilnl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gcfdvyhct.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gldbvrcnr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gsaqvmlho.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gsdtjucch.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gilpfqieo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gfizvapnb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/giiaxemor.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gldsydjzy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gjmbpjhvc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gaufgncbg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glkjbqgaq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/guljlvlzy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gewruhlcv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gaybmbwte.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gfefupynk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gtlugpzhi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/glkikmclg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gvvcjxtzy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gdtswctnh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gzieedhpj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gruwhjcqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/ggytwrqbs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbqcubqze.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gxffizopq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gztsbkpnp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gdfmwqpqo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmddnhs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gavemvesr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gchvbfamq.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhkpzre.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gopirsxuv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/grnnnxscg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/goyyohkwl.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/grrvoozsy.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gfjbfoboz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gnnsctatu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gdncddxtk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ggythhqmp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gscunqmht.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/guixqgzdh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gxptzetxp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gmhnkthwi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gsizcejfl.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gokleojgi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gsycnfppi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/guvsxhgvm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gioaakrtw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gwamhpqez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gyiwjtnmg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gcjygjcdw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gyuhbnyzh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gwvzhqmae.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvjrkmbrx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gikbflbey.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmcdocrhb.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gbrsduaop.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gdwfucsdq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gztvwkdsq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gmamdhawt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/ggfdliyeg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gbbrcvcrs.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ghoivtwge.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/grlivapuf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gppceefci.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gbmbwbtxw.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsukrelvm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gduabbiyq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gmdvdtgni.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gjdhirgzc.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gukvmqfnn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gwfcodynl.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gihylzlun.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gbwrkaygn.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gvfzmyvhf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gvnagccvp.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/guzvqghia.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgexcvb.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gfeurnstv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gbiomgfcj.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gaajmsdrv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gojwjidjb.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/grhisrrph.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gmfpfroyo.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/ghoxedpqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvaklyecv.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/glqizeqny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdifjzqds.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gvzhvuwft.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gdnwsvijl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gsojwiwdx.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gygywbvyr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gohpgaawp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gycezcbnj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gffmsyrtz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gecbchxkr.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/grtjltovr.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvpflfokx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gyhhzashg.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwstozjuk.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gomtxlkcd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gmsdfscbq.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gltobicny.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gqksmjloe.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gtkvtydxo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gloaqpgww.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gthwpvicj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gjgtourzi.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gcsqrysgj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gtqnrovbn.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gkbgcowhv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gugnlobza.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gimqhuofp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gotzwsmbg.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gkqrvvloe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggvbaituu.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/grhtubosm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gffvfmjwr.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gpieepfbb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gomnkdbxe.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/ghypnoxwx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/glruoxbbc.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/goadubgcn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsmpdgsfq.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gadblqbac.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjieqwwrl.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gidzzxxer.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gmommobeu.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gmhypresp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gcjpwwmfu.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gilcvcvfe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gecngomqg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gsrxexbyy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/grfouvmrw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gvafyneqk.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/guurcgleq.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gmekjxejp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gptrrdvdb.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/galnsyxvu.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gbxrftduv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gddagnwpc.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gyocsfayy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gkiuzvyfx.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/globvctvl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gxypksgob.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gedgzjuep.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gbntlqywv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gkhwexszb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gkqeefmmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gabadfcky.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ghhvaamze.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggytlhogb.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/glyjtbyht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gpzmdtibn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gxinoktdw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gcmavwoab.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gcdanpfft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/grpjaerzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gboqsouyj.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gvbxihvmu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gzgkjdhuy.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/godgonhzl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gvrlgtowh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/ghxhnhcie.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gicjsqcqn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gselannnc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/grgckhiql.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/ggjdcjzsv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/ggaacyakh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gniwvtlof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gdqwwdzut.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/ggqwzsjch.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gnesmlisu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gddmyemnw.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gjfjpglvh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gddckgmfv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gtgpmmetb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdimxqtb.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gvnyxxnsn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grhzotdyl.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gftjelqxs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gybrzqpbw.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gozzbjkwt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gpuladzmp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gnpuzrjns.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gnvecksew.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gfjaavmmn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gwqvtfonp.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/ggwjfkrpk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gihpphgxx.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gapoghgfm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdkmxpsjc.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gotonaetk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gysogcphp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gvxzyuuif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gmehgbhds.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpefunqch.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gcwwteutq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gmfzgrxrr.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gynplkbre.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkqzddf.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gjbrwkffd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gwsopfaee.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gnymniara.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gofktzwyd.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gqioejmwa.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gptimttom.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gznkqdori.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gtfxpjmbj.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gehduuhgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gqhalmnxr.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gdupzkihp.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gygplfsrk.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gtsfxdzfe.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gvszdfkoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gjqnilunq.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gmzpluarh.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gvfdunbgp.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/glfoequcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gyokmrxtf.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/giruemlph.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gsneipihz.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/glbwlvxfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/ghhtfzpyv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gyfoolejk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gdcccvctx.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gfwzgffzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdabrxqfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/goxmonuve.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gblppiclp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gvxmvbxwz.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gzrbcrlsf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/girrhzync.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/grgsxlqfa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gvimgegnb.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gnnvjbmna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gfhnffcxk.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gdvmkznnk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfvpvuirj.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grdnpjyok.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvvrqactz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gmdboeguz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdnarsmfj.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gokdlkwfv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjoodqa.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqkeafy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpslwxfix.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/guonppicq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/grhhrnyei.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gcsdbwfqb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/grjtvyayh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gjqyohgmy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/grbavcoqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ggoojwrwq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/ggpitqdez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghxcihgpn.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gamwrjalb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gzliksagk.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gxzbecuoc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gsfcojfmx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grtxafzxq.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/grhndmnoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjecyhjxv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gpgpbcvll.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gvlxzauwh.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gvhpqjxbn.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gifmivmgy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gdnhnscus.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghwnlhnak.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gekoqrzah.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gohbpnfis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gvmzdaurb.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gpefdiukr.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gtghlryts.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gjwxybtyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gzforfxqd.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/grltaizfa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqmwrxmjx.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gflxqotoo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gaxwrsmmm.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gscxudlxh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/goenvyaba.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/giwlvduqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gouczsmdq.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ghscgnlaq.sHtML


<!-- 参考信息 -->