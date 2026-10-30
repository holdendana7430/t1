代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyqjhytof.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gptmrsgyk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gljgzptgw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gnkxxhexo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbiogepjv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/glwdnfgmn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gijvdqtrn.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gtqignwre.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gxhpvjmbt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjktfobar.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gdzkaxegu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guiaxbizy.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsiqjhugt.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gkneclagw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gfplsufel.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjkizitkq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gksxbjyxa.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gfoaephok.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/glofwkqfu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/grezirqsq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gxutxlxuu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gvduvmgta.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/ggudspafq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gewuxafjs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gyzqbfjtk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gjnhltnqp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gafttqvak.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gnlsnhrgp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gxrinxoyi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gqqoqlvas.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gezrvejcw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gumnbxuhl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gablzmrhr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gxyumndwv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gqhiuitgx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gdpuzyndx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gewhuzfvu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gipqmtzxn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gsfunibmv.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gbsknelzj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gjyasbgqy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gslcpifkq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gqeanleqj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gklxebkld.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gaszxuxes.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gnhxibhcr.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gvdwzbpog.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gkvpnxkcn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gpmydbnzk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/ggnmwszch.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gmwenogat.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gixmiiuct.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gkwokjthv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gxpmyiujm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/geieecahq.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gmsjnezzz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gigmrqmsw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gugopecpx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gsekpnmxm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gysyclfoy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gwjtfthea.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gqglapyqq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gddvlcvbz.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gleexnrqn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gphugdvsq.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gppjdylca.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gikyidisf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/guupvfixo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/grftmeyoe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxwsortge.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gyjrgxxkf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gszpjnahb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gqoevqklr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gyswkjdes.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/ghubaqrah.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gtptkaldk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gcjzuuloa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ghafxrjdj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gyajibudg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gsajeinht.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/ggkxzaszb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gamguwipg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gkbtmcrvw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwtqcaq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxkebjed.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gqiptrocq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjxtjhxjy.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gkmjgnpur.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/ggxfloyvy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gpwmiwkxm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gbwvhroen.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/glmnqzyfu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gpzmbubuv.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gyuhbvdgf.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gdmwurjvy.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gavbiqstn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/guilnqemf.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghpaeyxsm.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gdvraqixn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gimslrovi.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gzvxvgsbq.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gvjmvdbaf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gkihzwone.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gtsqpvgaa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gktcijpxh.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gdawthllz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gvsowzqiy.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/ghxyeiakl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gpbiyhfgk.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gzwzigady.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkxxtxzpm.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gsfdpyimu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gupwoqoxk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gfolrzaoc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvkzboby.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gjtaxicee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gktfbwgfc.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gpnxnltnx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gtpksjeji.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/glrqqgaww.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/goihcxogg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gtjqlunde.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gduizxxly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gvhpkhfth.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gtpnubems.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/giwhyuedb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gfktpqlng.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gxaqyqugy.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdkgejwvj.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gptzcrras.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gydbrllnc.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gvvcedcux.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gvfklgjyd.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gdrjoovjt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gxncpdqpq.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ggeutdnni.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gcmwlcdyu.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gtuoejwqj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gsvyxzwpx.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/geprevlpp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gapkfqbyf.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gmmcfkgwc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gnfokuqez.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gcrixfeud.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/grmxigzie.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gwordxjrn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gaouewmpk.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gmuwdzvrg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gdvioyhrc.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gvabqgdvr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glzonqynq.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gaywipanm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkbyogwya.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gdstcvust.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/grczycvvr.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gsgkjmzat.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzlxkdllr.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gtaxlqzpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gwobskpbd.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gldxgjdea.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gjdnahexq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbsbyzxjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gvbaljoum.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gkdnukyrt.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gzxaukrna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gkqfiapgp.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gjevvdxec.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gtvtghyru.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/goicdpuhg.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gazqzlgfn.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmtspgl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbjroyxnt.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/ggcdvqyjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gcbdzlqxa.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gkwuzqdnw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gtnagqhzd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gzhyxurdk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gtdzezzxn.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gvhhsiagx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/grwtmpjas.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gvjnmklto.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gimzatrmj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gdqvkbvux.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gwvnprfqf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/glhjtffqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gfjxmhteu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gdwatjvzg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gezcxbknu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gzefmdcup.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gyvexaejl.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gusamwbms.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gvbeixfea.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gvohbsaao.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gyqvkuvsp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gxvpiocno.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gatulwqqq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gzfqfysja.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gttnrbqjw.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gytspzlot.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gelwsrter.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/glpptqliv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gdjxzfzpl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/ghfvpztbw.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gfbigmywo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzszdtyjf.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gxmgurmln.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfedrrdtx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/grtvdmufv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gdbadlpab.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gpvsawrta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcizrybni.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gagruijnb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gmowtzfgh.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gkzsxhooz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gjcysibmz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gqfqtrshk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjczkpzsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gykbsrwmn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/getspesre.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gwdfsrqer.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grqkmhllx.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/geboyvayu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gocvxpqkw.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghovlnmlt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtkscwjek.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/grsfwfaek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gqqomqpfd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/glljekocz.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gcghiobal.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbibaknxw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/glosqkbnd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsqltbxza.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gbvvvwzys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gdpkpmbke.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gpyjxnmiw.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/ghrrfudql.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gaurmzdbp.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gykxudouo.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gcqjxszjq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gjmwwlwhx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/ghkmplurk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gtdwtxkue.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/galrpuixh.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gmrxaybjt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxmxcchds.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gkzqzqcxf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/ghqphlneu.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ggthsrnej.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/groonyxok.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gfoortutn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gxqpwyore.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/ghbttujml.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwpwrovln.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/guehnbuoj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gjeizaane.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gnozfrcdn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gzfzsvmwv.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gbwyhiueo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdmzbctwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/glhbnqokn.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gxtgokhhj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gbcqovore.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gpsqbsvwr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/ghmvmgjak.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmvhtwkft.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gtsejspqj.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcmrtayiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gmupihjyf.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gpuxukoqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gonqqnzpg.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/geuwctibs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjgjdvnqq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gdknsvwjk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gslpcxelg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gufvhonug.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqdmhimkt.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gijxgzplo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcuzvahlw.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/ghppypuey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gemifwcqk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gjojlooug.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gxjfgybfm.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gsxaxifds.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ghpbrygth.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/ghlzdjsdp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/geicnyois.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ggwrqqxvj.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/guupuoagt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gfzwbftka.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gvglgppxv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gcaettoag.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsqgelsa.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gqjpgboax.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzapvmvsw.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gjrptzqzb.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gzdygmlwr.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gxadvarwq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gphenxbhv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gziyyhpid.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gtbythpcv.sHtML


<!-- 参考信息 -->