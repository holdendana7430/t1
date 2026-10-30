代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsbkbyfbn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gwrqywdek.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gbsfeqkaz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gkmoalanx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gbtdxpwdz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gjdjlqdwg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gvjaqtmnm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gsbglwgwi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gbmmggyph.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gmkdjnbmv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gmkzbyywt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/glyjogscc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gkimghiss.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gkdvgyhen.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gizaitibg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gycabyzeo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/glvdnhqkd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gcowfcfor.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gespouibd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gfzmkontw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gqwplxnew.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/glttllmhl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gpusndgnj.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/ghypgiwhp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gjxhcnyxo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzsihtcrb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gflebdoqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gdhrzcddc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyonjkgex.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/ghwaqujwy.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gjcphyype.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/ggpbeixop.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/graiofnmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gmcqvlech.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gyvugvkht.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gmmellmzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdtljfpvh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/glnwdovrw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gfcbmbahm.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gsbkwlvec.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gxbsyylaz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gudvgwcyi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gaacshqev.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gyftnltsi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gdzowzkro.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gdiztgtgj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/grlcdeqjc.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gumibwlha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gucwpfsys.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkuveoppz.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gqdnaobnv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gpcflhkgx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/ggkfbvvrt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcdhtmccs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtdksxxhp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gvijxcxoi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gucevzjou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gspmjpoqi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gjudagylu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/grnmlzpco.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gkmrpeynb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsnabfnbx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/geruezonf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdjsozviy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gbzbxpgla.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gpzjumool.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gvcwsnojb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gpakkfzpi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwhwqhakx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gurtplfau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gskzjcmlt.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gxxujhhug.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gjvxqdocx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gqaplaiaa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmyrqiyby.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gdllslkio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggucyuwqd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/grarhyznj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gbkormolq.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gkffcnbeg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdjbyykyg.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwjslqvfl.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gicfhbmwm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/guuwqsewk.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ginmsptrq.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gcneyqbod.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gfnvqklkd.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/ggzvctzsn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gfwhvhpsf.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/ggsicipiw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/glbsmbtzs.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/goahtysut.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gptayvtqp.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gjwtjwhfe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkugliwp.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gmrkbfkfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtvvkuuoy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gjgcitozt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gjlflhcxp.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gnakaphki.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxidncssi.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gkkxzekkz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gegucrleu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ghhxgsxtb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gpqwzdldw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gamnsynvw.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gdybgsxss.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gievmvpvj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gxdefuvys.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gdaguuvqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gbvqmscgi.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gagyxnmqg.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpyzdthrg.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/ghoasagfb.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcvfkjmje.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gdrddhdux.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gchxwdagc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gitpmosfx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gsanforbh.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gwssxwtmu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gdnmamapi.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gkoywslsn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtnjlbupt.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gofqvzipf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/glvpxlxaa.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gsfgrcyxt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gxswlpvfh.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gxuztxzyi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/glewatflj.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gfhhjjzil.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gnkwvcdsc.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gwsfnuirh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gauskslqs.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gpbttvncf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gggryvnan.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gczpnborq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwyaxiqpw.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gjbvuwgis.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpnredatn.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gfdhsmxus.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqbedbcnu.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gejhvdjzi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmlryzjgm.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/grprhcktq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gvqkyaden.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwgvtvcyy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzddrovxg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gtucleiic.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gdumrhggx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/glqtvoarn.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gbmrlwvuv.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gppqgxuwh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/grvzwnvfx.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gdnkqjmgl.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/ggcwcwlum.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/goxjtqarz.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gudnborjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grovsrjvi.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gdtoneifg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gtgzddsfd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gexlykspb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsdagcyqk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gmoprorpo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gaslbarjn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gvcmhjfec.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gqedeuvvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjmgneadd.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gwjbdbdar.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gjshdmuog.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gfbwcpyfr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gmwagtmnb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gindhjlge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gzmctptqs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcxvrpnsy.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gdsidtjch.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gnkxbvjcj.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gqwovnaru.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gfzagesjd.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gpwpzjrad.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gvehkawoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/goxcnafap.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdaqhcf.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gyfojocey.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gmkoavoeh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/ghuwiixvn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gjyhoporx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gcpftuicd.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gujljtyhc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gprbdnunx.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gzvyxruvm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gxlytptqs.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/guadqaegv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gezvhjibm.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gbcbuxsir.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gifisaxxh.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/ghwskwcyy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glooqlzgz.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glqkeblye.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gcugrnnoh.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gglotdhqi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gxsclwiwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gqeeepumu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gotpigsft.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gcxklkjcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvnhvtrer.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gujemqovg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghnvwtpms.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gqdiplsnr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkdzwszli.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gpzuqzwer.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gowpthyvg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gisggyuky.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gxxglobow.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjpgvwilo.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gxrvwaljq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ggphefocj.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkqujasju.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/galbzlyat.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gogdubtpy.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gtudhahye.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gzhvxkjqc.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gdywwvgum.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gcqbnlbug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gyebrlqho.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gueblgdxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/glydxrndp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/guhldhinm.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gbiyvzvjt.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gvqtdtryr.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gsrvgjggz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsjpnsy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/goqfxpvco.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/glsituptx.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gxdtbrmxg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gylmfehhi.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/genwyaewe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbhhmgzej.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gndyhnyse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ghlkowhey.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gyitsniym.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ghifvewhf.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbgdgfrzl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxpierhmh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gsdzqaymn.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gdiwpsxjd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gwahkkjoc.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gyiwhomrn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gklajnlvv.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gzwmkxxds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gqgdqdbep.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvxkoxpnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gucpgqqda.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gmjkrqavi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkvllnbuw.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gmialkdxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gwermkaqr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gjacxqsvw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/glgazfzff.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/goslyjhqf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goblgzzbg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gargucnxj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gubauljtz.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gxuxesmwo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gdkspgllf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gwgzupsvp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gxoexyhsu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gygxoazsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gchwjyahd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfvlfvmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gmsfcupkg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvmjqwdcq.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gwirvvbzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gyvmtcjlr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gypooznaf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gkidyunxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gazdszsns.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gcfxwaawo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guiakdkpu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/grllbppdr.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gagttiorx.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gpqjohwtp.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gmlwfnocd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gezrgfcyk.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gesawfnqn.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gwwgvmuhs.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gctyjlllk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gmagwffhu.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/grozbvffv.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gviomxhom.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtyvimohw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gzqwnpcji.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gtxqmzbjh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gxkencnek.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gkpqjsglh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gclklolus.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gyiqzojnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gtshbvsqx.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gfsdtnbtn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmzvvijpm.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gugoztarv.sHtML


<!-- 参考信息 -->