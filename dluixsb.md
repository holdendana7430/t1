代发 wailian999

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gfqrswkmn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gsflpkmse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gdymofeme.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gfaqkprxz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gxikihyuc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gnahqhrjb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/ghmtrrjrn.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gouncapsd.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gxclcjryt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggtijgqwr.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gjvvqtrxo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gligpxeut.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gkirooejf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gmwpldbtp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/ggqdoqoek.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkboldulf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqqouqjpy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbxbnxkfc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gwwmxwyti.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gthlkkpvi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gzqvvvkoq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/giuxdsbbn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gskzfjwji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/ghfpudjky.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gpkektypo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gaavxcfgc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gshbpbyqf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gtoojuvni.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gcopdelti.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gzsvgojyh.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gkezsuqbs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/grapiyafp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gdorpkxcx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gettsffgd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gcxskczlx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/giczdfhsq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/giftfoiwt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gnndzsqdl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gykqnfbfi.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gdhfcoivd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/glachlccp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtqintzvt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gavslglyr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/ggleiatbo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gvwroyosw.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqdkrdgt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gfgmcokhc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gcxepfszp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/ggchwkzji.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/ggxmsgmfz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gbldsuald.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gywrfxmke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gmdukhopq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gdiytrnqc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gicqugenk.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gkswylawi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gjhqyjqqb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gnyizbeqw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gjixrhnxf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfqltjtfp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gpybmkpru.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gcwyzmpwy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsvamccfj.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/guvehujgi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gmazepxpe.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/ghngbampf.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/goimikfmb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gzhsvzfqt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gqxihwiwc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grgvixusj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/guqzkqlyf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gbrfmvdvl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gyeyxoadg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gbtjmcbus.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gvlfirreb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnesdduaj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gepsrmisd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gkskudzkn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gxefghkoo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gbcspumle.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gwwgajwml.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gwbwyplld.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/glybipfnw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gkxqsfyzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giscquapq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gkgbbmioh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gngenfqdt.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gwknaoffc.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gcccvmdwh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gfazhumwd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gyxvzbayo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/grzctwttj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gkgkymdhy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gubbicnky.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gtwwswbuk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gayivptlt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gcqbelhme.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gzvpxwmfx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gcwrosajp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gtyxufsnp.sHtML

);
来源：http://wap.fehbvm.com/Article/details/grofjydmz.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gaksorwkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ggjstizja.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gbrpxmupo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gllujlqsy.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gdtrpclsi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gevehixqa.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gkytnvpgr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/goqrhavev.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gvppvmrah.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gueastkis.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gevbucglx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/glychpucd.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gibqygprr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gltryvbqx.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gtbqnchzj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gqgjnrinv.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/ggbzmaasc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjcnjngio.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gskdzlvur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gcowzrslk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/glaguhxwq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqnhksp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gntyxshjv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gdurpeovo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gpjxwpcbe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/goaaxpeil.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gnhdpgzgp.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gordtlegc.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gcmddjmgx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvdlkkakr.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gxrctakfo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gffehxtuw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpcequtil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/ghquvsndu.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/ghpttvqie.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gtstuaobs.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gxiyzkmol.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gpasajddk.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/goxhioixr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gxemkioot.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/ghpvegdhv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gnwplylbi.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gellmmgwp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gumfomxyp.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gjolofxmw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdhobkcjm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gtncxrrwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqbbcqpqb.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gcylswajc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/girbiushe.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gdvmxwzli.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/ggqvcwjfb.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gkdmheiok.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcgozefop.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gyuhsmfyp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggeflxbja.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/glwmgnnqz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqifewxfu.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gbhpbcjqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gxmftyrew.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gjeynflbq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gkhriouxo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gvkrshbif.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/glvsupqcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gokeprmzd.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gafkhadoz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gmoyatrew.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grqwbxhok.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gthynwtne.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gbnetjiwf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/graqdzhji.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gaozjctdu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gynaxfjam.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gwlyrqcgg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gadxcljpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gafazueic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gdsocwwhn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gydezswps.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/ghpndomde.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gzokuvwll.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gfygkgxvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/glzrqnmwd.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gcbzboqji.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gqgkdlzoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gewwbimbn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxamhjk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gleibbasg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gzmmucqzl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gyeljlkse.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gopzqnepp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gyukdplbi.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/ggozbynbx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gxowaieea.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ghvziywed.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmodlzqjy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gaifpggka.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gystwdmvg.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gnuvkljtp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/guxwwmuna.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/geblfayxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gyuhlbctk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gcibtqcym.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gdroklgvt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gllukxrpr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/ghfdoxskb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ghbweokmx.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gnuihwfus.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gizjbtwld.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gnmpmgkya.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gcgfhafio.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/grvzosvkb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/glyykfnsi.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gisypurnc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gxlpassrn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gsqykxzjb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gurgvxded.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gnfrmlexe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/godmdtbpg.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvozetwvh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkryapjas.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gbopzvipl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/glzyzavqx.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gjxzmhttc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbszmcwuq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gxjndzgxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gwthqalch.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvhfsipfb.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gcohwwxdv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghbltxtdj.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjmfhujtz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gebufxics.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gbkaedftg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/glwllhbks.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gvtmdsncu.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gpbhvyvny.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gddikluxl.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gbzzpjsbf.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gjajrziyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gczjpokfm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gktxwnyya.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gasgbvvef.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gggpxkcym.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/glhisrqcc.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gnmbjesyy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gwhaejskk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/ggpytpbbj.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/ghtcxvddh.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzbyvhrdf.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/ghlkjvbuw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/guxshylox.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gufmwqhns.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwzrsumcy.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gunajzivr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gakiwulix.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/ghtkuozxl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gsnkyvyag.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gjvebfdgo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzbvcxwbe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gbaqkbdxn.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gdnrwnmhd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gydrmlber.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gmbdeumif.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gebgathhq.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/giofztbad.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gicrtfibk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gtgdxpasx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/ghcpowzwb.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/grfbprnbv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbybbrvfz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggcpamkpy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzfincxpk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaskkdell.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guajfazmb.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gleqzjekc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbelrlypt.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gsopzzkfg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbsjwjprm.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gexwrvuhw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gkirbljgt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gzzctymsn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gbsoyspwt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gipgsvovy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gljpqrhvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gzamboxac.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gpcfiihmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gappkscpq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwoymsiel.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gvutvujub.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gexkmxqmm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gdlaylmje.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gktpmnhpe.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/geziubirn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/galhbmmlt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gxuswvgds.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/grqfgeuud.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxkonnvei.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gmlcugcsq.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gyzubbenn.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gmogiiwqe.sHtML


<!-- 参考信息 -->