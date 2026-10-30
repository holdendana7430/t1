代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gkyqmsjul.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gabyjjmzt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gapkoppap.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gpxmobsdf.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gvmgzyagz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/ghxhqlktg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gxmzoiusl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gihvesair.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwcobur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gmdndwjgl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gzervnmlu.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/grurgmxhf.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gjntuymxv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutzcaofb.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gdtbppwoe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpmnotbvr.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gmlyoqvkr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gozbnawqp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/goztvsdqd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gzzeggqey.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gnuajegbh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ggdpptmyu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gjomjzsob.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gnsgaojtw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gncdbsrev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gsafhtpxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gppdxljxf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gjbflmtve.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gxpwqjygw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/glscyedzd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gxfrospdo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gyyfoxpaw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gjmflxzez.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gjwtrmpjj.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gixusyztf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gevqjdbnu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gkvuqrlly.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gporwmmzf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gabikbtdu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/guselqjsr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gzmawchia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gznxyipme.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gwbpjordm.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/glcaxmgat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/girvkitgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gsboxeaxj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gtupagnkt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdyjhifyk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gufihzuyd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gniayrgyb.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gpjgzenth.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gotfnshwz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gjnlzzpds.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/ggxidvvzx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gczlxwlpj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gizhbfsyu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gsodeetav.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gcjhldnzs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gclktezlu.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/ggosfviey.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gzulwkwnv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfijmlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gkrmbwcrl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gvlsrmxhv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gpulsgktu.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gdvmlqqoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gspoennio.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gurputjte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gxdjeeknw.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gifurxemi.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gjsdkfqai.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gsdegqdlj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/ghfzsmgln.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggydheana.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gvyeweifv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gkkwurdez.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/galtcbyfk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gfrufawwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gcxleethl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/grsrnuoje.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gdmenvgel.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbnfxjsic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gamhnvdau.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gqhfqfzuk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/glwplhdrg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gykerntcs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gcwhnwusf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gjcjnvybc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjcuygsjd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gzsyswcrv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxidprkha.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gejxqxusl.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gtezpzkma.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghtmwbnqo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gueepjdcr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gpomvviaw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gczqlldjr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmeclmlwu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gtdztpacl.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gymqvuitw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gpwrqyjra.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gtsgfskfd.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/ghnrhpnzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gfwriyvdx.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/glhqjqrlx.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gihpioytb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gxszpbyyj.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/glahzcwhj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gabarlhwf.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gvgesyezs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gfpspjlix.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/grvbrbjwx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gbmylssrr.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gigcodubo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gozhgiuci.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gwiigxokz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzstqcos.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/ggfwyxztp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gbfssbgvb.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gyrpbjaea.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gsbhdzgcm.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gmoehrrae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gqbljknxj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gsprlxssq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gtyvkfvtj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gcwjlszln.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gtmkidqsn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gvydanknm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gnjqgdcmd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gbtuplxae.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gnanmpvxf.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gbqyslvrq.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/getruaqxk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gvhctebaq.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gqawfujtd.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gjwujxmix.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gafhemyqi.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwwlmkqqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/ggvqsxrvv.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/goftgapdf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gamtskpes.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gewcgttmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gtvtgpxsi.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gjarubace.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzacoonmd.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ghffnaikk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzglfjnlo.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gjhparnds.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gigfsojqs.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gxmuulugj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guutqqkwe.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gshgzkdqa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/ggffruiue.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gnyzzifah.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcedkatn.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gbmdxrhsg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdofuiraw.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gdnyhgkff.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goqdvysxi.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/geujvevfm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gujkbqran.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/golwviynj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gaqevfkjc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ggajerhwv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gozcmtkbf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gllfmzvkj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gsamekjsw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gkcssaxxw.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gxtakihdm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gwyqzywuv.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gnnwckxgk.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gsxzoskjp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gusgqcqxk.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gqcymojuw.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gslfwuhza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gedovrffj.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gpwnzzzmx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgzjtid.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gizvrajey.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ghwdlgxrl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gnrykypwr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/guheiifkq.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/giugsqeao.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gortiywgr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gdynidsdz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/guqtavair.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/grlhnehke.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gkacdeami.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gubhquuui.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/grdplnoqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gbwwqbeca.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/grvwwugrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/geifmfcfn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gzxfshovu.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gzliwbmcx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/ghfrphbqp.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gjazbcmem.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gjcopbfkx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gojqhgdcx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/getbqjsvg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gkwtdozvc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gtautjrpu.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gfirdnrwj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gzskjjyii.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gdigmsldl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ghoiaylqg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gmrcxxpdw.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gcrkzjyiw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gxjrssiwp.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/grpbuesmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gsknywkbx.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gopiifaet.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gsuakwbvw.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gxzujroes.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmkcvnbgo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/glazfingf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/grmjvzphn.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gtyuosaww.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gnpxdmfxu.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkpjdab.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gvfzxgvdq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/guxircyws.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gjzeptqnu.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gxlqiordl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggzzzqltd.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gdevulcvg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gznockoom.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/goxokrwbg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpwujozza.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gzjtwgors.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gnnmtoutu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbngflwjm.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/grjgoiwge.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmjzhnypj.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/giiheqqjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gnjbmytog.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gjhjsnqsq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyvxvty.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gvlofxvdy.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/grfpemaia.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gcppoirur.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/ggoxpvgki.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/ghnavvhlk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gynefixmc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gqlgnjrct.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gdthokjqh.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtaejhe.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/goypxrick.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/godzjrget.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gpdetaigr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gkmomcsmh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbrqbjk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/guvwfeosl.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gmpqbffbm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gxdnovxwi.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzqlxtwnp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwutkkcfh.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gysilytrd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gncjqxtlu.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/glybjqesv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gvvjoruwm.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjtkspxld.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/glcwmjsfq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/ghzuibvqu.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gumeqtlfo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gngyopfut.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/ggrvrlofk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnvqxtibp.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/guzcbahfv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gkgdvhlal.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gsakumkau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gvwtgnizx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/grtknzfgz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gluyxyhtg.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyeyazbnf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gedlgweux.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdwrliaac.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giovpbehd.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqyhjjccr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/giooycbua.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gyyqzjisp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvggmfkpe.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/geolcyxox.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gzabzcvoa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gqtpmowtc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gcagjllqp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/giuaizsrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gmmzmlhqx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gxgzjljej.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gipfovoln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gslvzqgwq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcwftdwvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gurfmywyl.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gzdksvaze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/ggdzzbnxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqtnficnm.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/ggiqkgdwg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gttyzvqqq.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gpdremrkk.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gbztcmbtj.sHtML


<!-- 参考信息 -->