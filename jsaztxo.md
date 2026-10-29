代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gvufqjkge.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gbrcjphkb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxkevhumj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gzrmzhbhd.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gryqxdfru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/groxmahpu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gvcqiibhh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gqffkjpmf.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/grtuwrkal.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gvalttztf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gobhtgetq.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gaojlqtan.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gbaprdqsr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grjwflglh.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gcpueizrr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmoazlaz.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gycqpphau.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gjocuekvp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gdgdthgqh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gihyeldwp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvgcqxjpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gugetjmlq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjgbmljvd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gtaabgvon.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gapuqcmmn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/ggqldjxir.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gonbfeaul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gahagmdwr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/grwlodnjc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gsovrgxsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/guaoklssy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gbqebeoxo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gdnycmkkx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gfrahhdey.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gwevgginh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/glodunese.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gnrzxmstq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gaxlrsjjm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gxamxbobw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gbcvwdcpj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gfvyqmvtz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gomglkdnd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/ghdrgoqba.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gatjfpmsu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/galeebnhh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmkyucpyp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gpphwgfkf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gstkyoiut.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gourdxlag.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gtzmqplku.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gxqbikopv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gklveecaj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/goihgyiln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gufsnlkcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gilysilps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gqjkdrjuo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gumsygmlf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/guumznlnq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gbvxdkhia.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gaxtxrikz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gauredfmn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gohinxyag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gaxbuuqvz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxxkcwnfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gtknnknap.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/grwnuajtk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gptnrtuzl.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/ghplxkhcb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gmdobqppl.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gebuazieg.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gkydrjgsm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gxahtkgyb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gznpypybn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnwzzwabq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gooovwhob.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gzmcqvmmy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gdbhkwqzd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/ggafcfdgk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gsnyfdqmw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gvtgyghax.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gtlcvqjai.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzwdmiglr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkympnyof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gmqzecmxh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gaiimbrnz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gkpryavku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gsjktmzed.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gpkmnibvs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbiaxntkx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gyfdzqbnv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcovmkbwe.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gewlqhxhv.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gxglruqlg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gjnrraiok.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/govfmjeko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gwsrjvopu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gmpnjpxug.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gmflhrefd.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gqztxgbfh.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gokiqlijk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gtkzdpcsj.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjyqptsln.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gwdprbqqz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gxwgzvuzo.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ggzzsytlk.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdigherxd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gavqlppit.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/glqqzrxye.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gdzyijkvm.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/goyxnqale.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gxfwkznjv.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gcfzihzwb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/guvjitbad.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gbetkyuhh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gbtzqtbpn.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gosbbunvf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/goavgduyk.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gopozdisg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gmvqzjasq.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gionjdddw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gggifheij.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gjzaeidmb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gxjberubd.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gyxkqyvov.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ghtrjyjth.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/ghcuycrrj.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gjjtbljdk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gprpisklr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/geywpnrld.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gmanjttlv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gihlxgosw.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gfyctagec.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gimihxvla.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/grwijhozn.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gsbxrhquh.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnsbbba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gvgwmhxjm.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gltltxsdn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gsbndnbtg.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gfuazcrey.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gzawdcand.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gnjivjiuf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gczhvjdlf.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gturludnl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gzsolvoxe.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gstjkdiav.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gcdavxhjb.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gilcywxly.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gdiovqeve.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/grogsaule.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/grkeutvsp.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/grsdxbgmx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gqelfhble.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gfulinase.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtzekukox.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/geqfrkvvi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gsjllurxp.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gjoxfnihs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggdicjrds.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/grihtzttz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/goniszodt.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gbsoinrab.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwxdywsps.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ghmwiifjm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gvejccstj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gvrklukwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvydwzgjj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gvxrsvwda.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gbmcslfnl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gqwzhibok.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gajcsccqw.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gdcvtzggi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gceynmddl.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gcckwgxms.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ghchpybso.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gbahojixz.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gobbjsufc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gbzyavzci.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gkbvdbdew.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gucafonln.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/ggxgzgevz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gjyjkwljt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gjbzwakhc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/glqvpdude.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gbxvabvay.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gbybrtcgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gnrgfdcvi.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gyuwtdcrr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gajhfkhvf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/guexnihgy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gnjrmkdgi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gkufplgol.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gktothbqb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gakegsupy.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gyidwlkzf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gxhrqlttp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gzorhspwx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/giqkhpgml.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/glugjfnae.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gorgjvssa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/ghtvqbsde.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gibccklut.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/ghjtijnbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gktjopexy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/ghfyvazoa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/guhomdypv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gcntvrjyv.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gteudqmss.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gfhexyffp.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ggtzopyxm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvolchqdo.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gynhnlthu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/glywpekih.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/ggnozqhel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gallmkaqn.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gmxiddsnf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gtzvkbkgg.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gnezfcbxj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gadachfya.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ggxuloplv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gvoktoixi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gzswcsire.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gtpskwqkz.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gzyyciezi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gczvdxepg.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/guzspaewu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gssusgkia.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/grfnvhhbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gavawzyed.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gsirhoeed.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gvhivlnvy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcytodnek.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gerspdiae.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxjgqpiom.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gevapovyn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gllfsnepf.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gephjmzpj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gxqebqxra.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/giewfvvgb.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gwcinprpt.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gnwsdtjtc.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gusfrofdk.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gykphzskc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhnpsapk.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gjbtdvltz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gqtbsckuo.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/goucndxhu.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gixintfmw.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gjfisngup.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gmrpoipxg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gwlynjrcr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gcdhdjflk.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/guwxltahf.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gmawzowjh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gvazooizz.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gaksmpbtv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gowfxfdnh.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gdatenntn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gydlhqbxm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfbeqcftc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glysvbrfu.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gnxqigqth.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqkbljmvx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gdvodoiiu.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gypkbpbxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gpenpfpil.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gfxlnzunn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/giigtcjft.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/ghodfpesq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/ggsikllsi.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gillrhgoq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/ghaaopuzz.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ggmtchzds.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzoksmkg.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/goeduwcgo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtiasqmvf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gvbaayjne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gztembryh.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsbgkocew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtphrlidi.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/guxmvchqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnuusmowb.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmyzksrth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/giehwdzpx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gfemvokcy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/goahcglft.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gojrohigj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gwcvyjana.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/ghlqhxdpe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gbpcaxpyx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdoxcfvdp.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gzjfendid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gfbpirwqn.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/ggpbruavc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/ghpzhnffe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grcldxzmm.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/ghwnmyvhu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghtsimbzn.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gvnmdnhfq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gfuxxhudu.sHtML


<!-- 参考信息 -->