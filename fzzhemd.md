代发 wailian999

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/geoxlbawa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gbdkunuwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gookzoyyq.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/grymloklq.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gxtowuwgo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpenyrwea.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gicrorxmd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsygpnztl.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/getcgmokw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/guptaeunr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gymcbanda.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gkbakyzkb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtkszldkl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gxynkbuyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gsfyojche.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/ghqmveqbx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gofqjwcnb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdbsmgrzg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gbtzvvaww.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gzmhgqnbb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/ggydwcpld.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gmuqwoysj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gkpwpyowf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbafxisur.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/goijlbxiv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gixmsuifm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdkbcffle.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gkwzkxazl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gzxhssfoa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/glqtewvjd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/goesmxyki.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gijzydmfz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/ghndpvynv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/ghfvconfe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/ghcftevcw.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/ghhokjxzm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/goskabuap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzseykooo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkkaiitwt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/geyizwtmc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gcoxopkse.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gvetkifnk.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gjauuspeg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gdkkggdsn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gaqfgsdnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/ghqxbpthu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gixboliuq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gbkjtglpj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ggdbwftct.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gdqyexlvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gfohstehz.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gwnvxkbtp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gzmpzpfdv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gfafdtikh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gufehybxa.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gqdsedzyx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/guwrtbfgz.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gkrxzhoks.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gbuwvuurr.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gqwlugdja.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gwryfsjwv.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gqbghngnr.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/geqdwyfac.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gapupbgvi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gbewemydj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxjllzfes.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtyviujey.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/guiyagxvd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gldbfzqpy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gvirkpoba.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gtpifhcer.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/ghcrsssny.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gmnbftupv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gkhwhvoat.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkyysqhur.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gqndawjiq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gbihmnrmp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gwpmjwqxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gdfisrbpu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gfxajzhaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghvlzzhwi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gfclaqoau.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggwptwzco.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gyfxowzko.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gufwosvwi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gktihkush.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqbwwygtf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gmopferas.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gtylddayb.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gouilqyeu.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gsptmknvl.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxcbkkdyy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gdzjiryth.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gdidkjtmk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gbcdtexxy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gmdfjwdqw.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gthxwsbfr.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gpoycxoij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gxhfllvvi.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gykecbiwz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gpcxcxsfa.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gwfeeekfb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gyevpqzbz.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gezxenucs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/geauzmpcs.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/grnnnzlye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/grptnvgdx.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gtyiayzdf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghovxbcbz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ghsmkippz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gdtghzuzj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtznjbcma.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gnpsbehnr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gthzemtyg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxycrwsoo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gzjgpfazu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gncwjtneu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gfazpdccg.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gstkupkan.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/griwvzltd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gdqngmydx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/geasrlhvx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gcngravgr.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gwsceeepx.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdmgvoeco.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/grifboeya.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbtbjcypg.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/guxahzeah.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gxquqxwrk.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gsrksbozf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/grwxcqikn.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/geqsrcitm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gdsqwfbey.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/ghxegysaa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gfgqctqoh.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gyzcyjplv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gisytiyjc.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/glejbwcrh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/giymqdtdz.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gcahyuzmz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gjqnwvyyr.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gtfgrpxug.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdozugviw.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gltkddjct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gokrcmfqu.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gxgrkgbgw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggbcxubpy.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/golciivif.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gfjhkcxcn.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/ggypfrpeb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjobuhiww.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gutcnbdzv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcpqhvfqq.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gtpjzqjdv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggkdizixq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjhsaczfa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gkrqmlixw.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glnyaafar.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gdykfzmuz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gcoknotjv.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gdkvtarrh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gyxszvxcj.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/glqiowwdg.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gueunvgig.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gnrorqbal.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gmdyawfbk.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/glvfwjftj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ggmznldlw.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzqjburfg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfwbplpxs.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ggsghoxto.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gxzpyxicm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gbjdftpcp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzispefec.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gwuvebnrz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gvgvjrwbd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gmovijkye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gwexefzdr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gdoipolhg.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gfsebbmen.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gznlvqblf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gygjwyhhp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gsybrptqf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gxdvvgdtg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gesgkmbph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gdedqgbxg.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gidlqcnzk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/glycpxyub.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/ggggjfksm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/ggyhinxgs.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gviwhbqvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gsqxqxrlm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gdogmryyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gfqsxhxro.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gzvlnnszs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/ghyhxhsqh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gbxdrwbvx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/guyqccpnz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ggjvwtfad.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gdcldcfhb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gniulpczr.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/golavoqgp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/genvmjdhv.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gzkizznky.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvnpsnary.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/grlcgdezm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gddxawbub.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gdebjmtvp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjktykbkt.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/grshhcvdi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gxbrjllkd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/ghqpshovd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvouawnsf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/glrkohhhy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gabcgvsba.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/geioczhiz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gojevazec.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/ggcvnyqwo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grknyuekq.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gjyzlavwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpvwdjnvq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gtmientmb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ghyrfrnlb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggpuwenih.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/ggpnsdfxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsohpnuph.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gwxepktwu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gdgezbtka.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/goquiqabn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gkhgzrdcm.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/grhsgwbsm.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpqcgpskz.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gmnilpvub.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gbcjdiqfg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gjdazeorb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gfeqkkbol.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gzxuddsxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gtnsucfon.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gaexperxe.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gfjwzigbo.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gcjujjeih.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gyszeeifb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gmqrxljeo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzpfqum.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gvazrryia.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gauvlxewr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gklkuedak.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gqclzphdq.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbpsydizc.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ginixdgae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gmiuuvyph.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/ggoumqajz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gqzfoxxbl.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gperxhntk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxjtosoim.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/geeqkuiit.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gghsqvmgw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gvqcyrred.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gimltzzze.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gknbampno.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/griwscqmq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/glugwvvey.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/ggxssxdxm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gitehfvbn.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gqvtndrht.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxskqesmn.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gtosrlgax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/glqtnfgxt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gerqhjdat.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvxttbujl.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmqkigkpb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbegvpuyu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gtmriqmiv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gavtajcho.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/glljpxbfw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gpycwejfl.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gedfclnro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gnnwzqaon.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gtzfkwyce.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/ghlydhtby.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gqfbeakpc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gpjjjgude.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcsbvkhcf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gzejsdnrj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/garqyohow.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gogrlgqic.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gjkstdllk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvsnxnyxb.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/grnsemwef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxibdaqgs.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gjztshske.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gnymipqys.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gbpzogmur.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gxfcjcmcb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gxrrnezgk.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gdfcqdgyr.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gmrdmvgrh.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gmzdowhoy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gzeymiprh.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ggufamzmb.sHtML


<!-- 参考信息 -->