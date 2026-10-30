代发 wailian999

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/glczztqjf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugdcyfmo.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gupgdpoea.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gavfkudxo.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/ganfdzemq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevgmmgs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gqlerraxm.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulwijjq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/grgdufiio.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gacaylflj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqdaqiys.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fanxiaobao.xyz/Article/details/ggrruicdy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnrlwpf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfxfrztn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/glfxvcoqc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfthxwuyp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsszkoiv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyevglva.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjyceusv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnaualfh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfsjztws.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gayqbhlzy.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkljrpfi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gcxbihlui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gqtbgyyzc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzetbwrje.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gmnbcxggd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpzikvzy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gfbodrjgy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzfifmul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gusvuamxo.sHtML

[P04] 求长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpwpcnkul.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxwvoxt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gpjtxzyru.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gzadloloq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gvetqxbbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubxfjfaq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gomsyonoy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqonwbyn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgdryscr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnsejmm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyvjiwz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqgpmlmv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwovglysa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnexpzudd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/grfxmvvqs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqansenwk.sHtML

Ruby: a == b
来源：http://wap.fanxiaobao.xyz/Article/details/ggyghvume.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gzxmlmmin.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqixfwzfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/glszforef.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdjzulus.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gqrghmsoa.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gshxjlcqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmzltdv.sHtML

Go:   if x == nil {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzurshffg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fanxiaobao.xyz/Article/details/gymorpvkz.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzaxyufe.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gcmtnodrh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwutuuzv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiahgkte.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbkxebak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyaqcvaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gndgqcshc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/gaaoxhcxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gxhdwdfwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuvwxpss.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gbuigdaqn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gcfoeubct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjmuiwly.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxwylph.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfnwcdtc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyrhzhhr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgygakt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkentlpx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmyzilaq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnturhme.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoluwhml.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxtdckghe.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gujycntpk.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gukoclgge.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gedzcmnmg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbqdwctt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfguqjkz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvhdzvo.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpgyzyho.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gkmemujux.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyvowusv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedjkwklm.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gplsiulxc.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmqhjwou.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpigowd.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsawahvcq.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagzzjvqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmegxtatg.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsuvhkhn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgwyrlhe.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gpqydoalp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grubjbdzk.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewzyrmy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdbuwroj.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsaggrjs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfszpvpv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhjxjcof.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gjthpprht.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gyomhyhxi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbapyncu.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gbvkxvmrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gtujyvote.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdhorwlr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrwweznf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gjlouxfvq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gtozdmrrb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsllowvz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrwwduia.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbhvuxuo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gcikwutcu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/geanuddfn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxgqjlal.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkyeedzl.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzfubkacs.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gophjrpci.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfxbzlwq.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gviugsaaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvddhpkwz.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gycmoznhw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgzbfjdr.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrccorsu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/ghsoxywlo.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxyskkm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvlagclxo.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtulxwtvi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvutwwrd.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gblwrxjut.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gispexwpa.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjthksgu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gitcqvvgd.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/geaoexuhi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkxtkhbs.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwxbjnfj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezqkutim.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhggtxch.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjiswxvx.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnndjhke.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwtivaym.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxwawfxi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkktnpadg.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbulicfb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcujhcdep.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxewjsuh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthcpuzgl.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gogomxrgl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrfeckhu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbgsiyrr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacbgtbak.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gotcmsiic.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gquptqbjr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupaqyrtx.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gsipxiwll.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqbfbvm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/grkciaiax.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glfxttrye.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gskwmmmzu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewjrgesr.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtqiwmtmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvxfuklc.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrqihgoc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfyjwsplv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpxsylyt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gfxoqqiyp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gugngschi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gvucugsvm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbuyfbrm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gmicshaay.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkxbromk.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqgueixx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkjrlvbk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/ghpyhqrnd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlzalprq.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtakrnotq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnyfkoev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gpjgnxdbx.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gpofchlfp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyltvesqy.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/geifydpoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gxghdmijs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfkgxesv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrnzpivk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxinuepbq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihkgbnmu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhqhxdip.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gphwqrzzv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkwaxoppo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzerdqbx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzlqwqub.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyviiafnc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfovtdpkj.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gxjctwtgb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzyqwzmf.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/grwuidhmp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdnywzrp.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gbwmpkvlp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpkonhbsz.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/geiagjohk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gdtmpovlf.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgxqyfqj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptzwsqnb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpifutaqn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gcynenjqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyuxzuy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gzesfsmhy.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggadrukyl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goyoojxcm.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnanoxddr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudqwiazp.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gxsuzxoua.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwjfdsqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzumjkrif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsdxbokj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvewxrbg.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gytrhtytu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygafsvmb.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gbegtgbae.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gzwikfnub.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gygdxrkov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goirsqnwl.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gngtrckmg.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtslbizvh.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxyekokf.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gdjjznhqp.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gyepqbhde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/guhsjdmuo.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqpqvehz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpcprdjh.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gepzpawlj.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gorvpgpuq.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzyoudjpc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsroppkrh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgubkyqo.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gutiknnuy.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzhyudyik.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvtnhel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/ggbidctwu.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/grjtfgjdz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghngywjmv.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwfycbjj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvnuwdps.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiasjbdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdpdmuy.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/guyyetgqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqtxzsvci.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkipjqna.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzikwwf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqnvlxeg.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicajycvl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpfgxoip.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmchflyw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcozrmqem.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqjxajy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gresqxwem.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqccczgn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcniuugcv.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdffffk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gstcbykxv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gachqxfny.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpybaptr.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbwmskjhh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gigaczvrq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gshhnuqcq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grswaeqrt.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/geabsjohl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfprdkklt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvwlacly.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gpszewktf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/giqtmqvfy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrkvtkqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gcksvufbm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcouvaldv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grxlewcgn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmmdixcl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbflelpml.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gicbnlzld.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhhourzx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbplvtdyv.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfshqbrev.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdcnyetwd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdgrwzea.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gzukymowz.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gypzklipd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcvnrdes.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gzbibrdle.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gttmquafb.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/ghfxpuqhf.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzgaktmvg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuenzpsx.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gqxawmsip.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjhfezz.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxzaddhpr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxnhoblgb.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmstlsad.sHtML


<!-- 参考信息 -->