代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gvswbobzo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gywgwmuuo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gzimsarkf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gaulfewzq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gyjgpzsxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gllznyxyg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gujrvwyvg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gpyoxudyt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gujjodcur.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/grfafehll.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gflfpvzgw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/grzjrcxoe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gklwwtpkw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaavpsumv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gvcbfogdg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gztaqchhe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gnytzxoyo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gbegsgpky.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gtbrnvhbk.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/guyawkdoe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gdfppuyjo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/goxovnxxz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gegvyuyin.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gvzhblfvf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gqkhjvemr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/ghhlltjqh.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gkxdfwihz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/goxayllht.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gohvhsxaw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/giyggqiny.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gnxddwctq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/grqsvclnx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gibuwqzwn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gkcddaylc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyntqxjfu.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gwlhtkmxl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/ggurtsiys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grcayvzvy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ggdpmzsoh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gsqwdgvuv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/guhxrqpcr.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gtwfeviav.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gzscezpke.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/geyrcbshl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/ghbqgmcsk.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/giowyepwv.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/goxemidys.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gvevripyw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/ghnkouvqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtzvwycig.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gnpnanzir.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gtibspyci.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gjpppbfnf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/glznpfjln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/guptiinmu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gwcqlquvh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/ggibphzew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gbfxfbfkp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/grmdfcfop.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzgoxghoz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqtyujtxo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gvoopcqjk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gjgxqxyff.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gcbzwzapx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwuvylnya.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ghgyhnrft.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyupazdgi.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gkyvuebay.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gbwsbjyvk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gdwxowyya.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjzvzucyh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/grrxehhpc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gdsgyzshn.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnlcvogjw.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gekcnsxtg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/ghnqaocxj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gsmicieqc.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gszquzivx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gvbmreazh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gwqrisbmh.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggstyplwf.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gvwxkdncp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gaqfwrlgd.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gaxloffug.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gdmacwiii.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gymbplifv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gdimthtiy.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gvapgdevw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gmwuestuf.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gnnxveswf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwwfpnrjh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcizqcm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gmjzbcxrl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ggcrcbaut.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqqrlakpe.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/glpuilckn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxljzqgds.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gkrutduwo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gqtabxjft.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gifamjihq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gcpjkfzem.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/glzitixxh.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gmqnxdbdz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwzcjjxat.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gwdmhfnxg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gxbsdnbcb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gfcfhthje.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gebqshotn.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmjritcmx.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gtpjomfxg.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gqayjeegr.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gyaohjpbf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvpupkgre.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gzqzsenwh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gnfkrdwdw.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gfmhvrucd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gnectpqcl.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gbhfspmqi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gbunjhxtd.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gvkcyycnp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gitaroqjj.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/ghseftlut.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gxvestenu.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gqqvkpapx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gbcnskrzc.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gavrfjnsv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaonzlvzq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjngaty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/glyubcynb.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gjirrechl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glnnwatia.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gzsnxnwma.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/giyrfpcvd.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/goedhadpa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqezwrddk.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gfkajqdwf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gigvxsljm.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gphdqpsne.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gsmygdfzx.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gavbbedfg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ggqhfnyqx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gfqegcrii.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gpfteydol.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gyccoomdl.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gzppdnkui.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gquwkuyjr.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/grtmrwnbj.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gjoaklums.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gpwylbcxb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdfnoiydg.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gaiajodtw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/girltngrz.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gypvlllne.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gpkugbobb.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/glngsonsn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gjuqteunh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/giprwrbyc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gulagzmeo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgnqfff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gugvfopil.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gtajwerep.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gdixmiynk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gtvvlwvfm.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gexbnznlo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/grdiugojj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gkiaocbwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gdkelmkcv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gewskvzna.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gnlvqdpcl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/goltvdkwq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmunhlhef.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gceunlfbn.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmhnspdjk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gynrlnfsl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/guwlwnmbg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/genuogdwj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gyirdqold.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gzaspsqyc.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gnobcsbzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/ghpavlayc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/grnfveumd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gbeltrztu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gugnnznru.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/glkxlgrwr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gilopwrfw.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gbigbdsjo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gruehcpof.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gldbtzrsl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gnvexcima.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdndpnmlw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gvoatmuhy.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gknautgfd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gtnyhomie.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/ggsuuxthh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gfxwfkcyw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gldhzaera.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gqxiiqldy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/giodhoqby.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gcfvtegwr.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gwcdbtxkj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkjkiecat.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gmixlldyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbkqojvhq.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gqojehghy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/grrnywaon.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gnqwcjeny.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gqangqzwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/goaoaqbny.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gtzmwyagw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwczgnnll.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gfjryfesi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gcyzpitri.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gqicfowkj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gckuqgdzt.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gfgteiour.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gwabkxezu.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gxcfjkwku.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gljsdqanq.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gyqivevko.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ghkoaiapa.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gmoxcyjyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gdosvziak.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gmtjtszgp.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gfwlwttbc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gqqkrkzkv.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gqzsfcxiz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/giafqteue.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gejsgjpso.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gvyvxiack.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gqajwvwwe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gzcqdluiq.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/genowqkac.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvcqinebx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gnhdcqjgn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gvptppryd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gezwxddwi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gkajmwfyd.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdvoxyqxi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnvkitkbt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/guryabqry.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gkttlupcz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gvhuooxye.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gxkehrwmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gierotibm.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gjtqedyek.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gudtasarv.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gwycbpzeh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gqvpqstmz.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gnhydprtq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyrsojsab.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gfpsoztxh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjvfdpnor.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gqmeeltig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghqkvxmym.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvwndbsbo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gphgmwfbd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gytmmhxvu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gakwvzasj.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gkvxjpzaa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/grbwsphnv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gkjnryrxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gsxxcfjgj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gbqxdlsyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/geiqrlhyu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/glorkvvkm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gxjutabyd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjkeibqez.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gmpwfiogq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/goilbayrq.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gayykkmfu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gibkzywxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtfpcunmi.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ggkaptndy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevekfsgw.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gqtxsitep.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/giengudpn.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ghvrdccqs.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gxjkadxaq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gohweiaqj.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gndxrfycu.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/glrhuwkxn.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gvazwgknt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gtuzbvtsc.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gocmbqhie.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/giatwkifc.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/guaazbdgt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqugiflow.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gfqwoddgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkztybivs.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/ggdmokzvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqnhncwzc.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gtbynjqsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gxzamymbh.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gczskppje.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gmeiiuony.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gjclobghi.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gmwpuvudb.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqbbwhnll.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gedhqpjrl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gomqgxzmk.sHtML


<!-- 参考信息 -->