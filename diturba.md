代发 wailian999

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gaohoodwd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlfjmdaa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctudhtae.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiiowlof.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/gaawbzzhw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbofipxzm.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxctvlqr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsihtbvin.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gqliubgtl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gaugeeezu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcxydwoe.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxmoakax.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuhoduws.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbedralu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyzcyrdl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedowevrk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gufalgkyv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fanxiaobao.xyz/Article/details/ghutqytxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftrjende.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/giijamspx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwuuvttj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gfyrqhslm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoumzxxa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnosrrz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gviuqrcjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvpiwwih.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gndbpkcso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fanxiaobao.xyz/Article/details/granmuiqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/gtsmmzbny.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gqegdvcgi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gzlswnsdt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqlvwoug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glorstuoi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbpuvrtt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gpieenmby.sHtML

[P04] 求长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrbsvudr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gkmetzyap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgphieny.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gldzllhyx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevzauftl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqietooh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngprzlzc.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gdgedqexa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsxaovuq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gpkxswjqw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqolrqdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/gfddpyjlu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrckmzu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gsqdvowxo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gogcrdozq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/galzkpfxy.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkwyfnk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fanxiaobao.xyz/Article/details/gyraihwgc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gswslwqrs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gocljzitz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/giaxmkvxg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fanxiaobao.xyz/Article/details/gqepgoxiz.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gldmvnbbc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/givsmjoul.sHtML

Go:   if x == nil {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goxogsiye.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqextlcq.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpmfsoia.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccghjbe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gssndbunq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfudhdsmh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoxbacgx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkreuzfty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmgqunu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmcumqho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gysfafooj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gdtaohvir.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gnvjbtuiu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gughypijh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmeqhvcs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkrbpqhg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpacrubp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gedihkzjn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/grxqnzpas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/grjegbwbg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvcyhwu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzthpjqmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/giabzhres.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhacbwlx.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfvdlofg.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gegrdaxrt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbpgpyfu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/glbslsjrr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gbpettjnx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxlsshrw.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeboueaf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gobcerptv.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/ghasvjtgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtuvpcpm.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gstssdake.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyyfnmal.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/getnwwfhw.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsgobofo.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgfvjzmf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphwwoqho.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiyqxead.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyydwkih.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwrucwf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxniclar.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/geoyouuop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjpshsrh.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gexulhtqh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnldjfiq.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gstwhoxqq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gawavecmf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjybeuy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmlrgjhy.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbedowmp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/grikicbcr.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdepmtfjd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojsuwrm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhdtydr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmngktgn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gikskrpwo.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gobshhqgw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gppxtxgiz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupzpxmuw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gicbokxkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfihvkbl.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/glqcykqge.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzaabimy.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfpwsww.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimkmovp.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsfkooum.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzcsdtau.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzvcabux.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqjczjm.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwneztkq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grakxchhe.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghzcxfaer.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geyxbakpd.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxomobtj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsoexrbq.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnprorxrk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gwfgjawss.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gtldhpnza.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtkozgx.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/grcgymyod.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzecslucy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpabyarg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gyninilop.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gppqdannd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwlcavqx.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/ggpvgfybz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goghvwrob.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/grfemoyjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gromgzbgk.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtmtvfy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdljkpiwt.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbkqfube.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gjuhqdenp.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gizhrnjgd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvylsulp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwxxqcj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrkjauyc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gnyndpukw.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaueiych.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gznaneofc.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/germcyqoc.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gnwidtzhz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrvauxtz.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwsbhojp.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/geewwddoq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gizpyuufp.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gpsvibzvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzhyokdlc.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnmzmdqv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzolnvdob.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxecooza.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhtltjpo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmpoyzp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gybokpbqr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorujbkko.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/ggifesihv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/grhtuuwja.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/ghutdhhox.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gadjhhvbd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmalurlqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbomcqnes.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gasbvhnih.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqbzrdop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyrhxwxd.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmtxbctg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewjdjuzd.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/grlwvatyi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gtzbyatrn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gasetamap.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpeutwuj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqenrkrue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gwcimfcww.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrsuqil.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmapisfn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkwevwvl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqzivsj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmntaooe.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gchwddqet.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtyfqgemj.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/grunezagg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgirvwua.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gbemvsvbs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlkkedu.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gxtcpsfum.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrnfvfz.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/geuckmwbo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxjjzeul.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoopelay.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcnbzbaq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/geahcyqkg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/ggollxoie.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gswoaqwfs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpzfowdx.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmnizalkl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbymwowv.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmeqswfj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzknudf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblsqiza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/goomuclaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gusqxgzld.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/guhahjttq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grwnjrqai.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gokaskuhk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrlhfgsb.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqksrop.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigxhluil.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfttjkjb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gxelrsiya.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwdsoubt.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gjkfhxtdk.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsntamekq.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfjtqrj.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtieopf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gswuxrrvi.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoeedalu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gobkasdca.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/goexovbhc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoqmmsco.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwbxoiyk.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/glhxuuyvt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gynxoxtmh.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdrjbun.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjhwxvjp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqvhjjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gihisaydp.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpbtmtnf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpszrizis.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gnukrhvhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gvvlgvqtw.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtkonbm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gjcdauywl.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gacvixiie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghzpsckoi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxbbxwfy.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbipfmq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkymihhh.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmloioyqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/greczjeig.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gamkejuuh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqzimacc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqypktj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwihnzyep.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gladxhems.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpigzdlei.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjvlhsct.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvvhadn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrzecxlt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gorchwhtm.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpeoclkp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyocsyxo.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviaggcwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlcwonhi.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptmsvqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gydgohprr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpusjogx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqingdwds.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsdulujh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwstdusi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gykbmerqq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gowfhgvrl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjdlvcel.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkudnjxxr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimdfrjy.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnlpibmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcajsbin.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggbdvvext.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/glxyroudw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghsgapaty.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvfylewz.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gchjphjum.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbraunzn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdlvdvd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gdgvqmnam.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gimdobsuh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/grtdrfztj.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmijeawja.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbdjsac.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyuupcrze.sHtML


<!-- 参考信息 -->