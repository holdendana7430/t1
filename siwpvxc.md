代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/galxfdagq.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gsitnzuod.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gfcdvkraf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gtkpicxxr.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/grsjrxexg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gagefkayo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gwqpzdtrs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjrypcaoz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gizpygluj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gujnnwkux.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gzohucyik.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gzsmlvqza.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gguiutnds.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gfglpjggs.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/ggskddwgn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gffkzfzbp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gdxidsluk.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gapzbyvoq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbwjajoli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gfjdrzjeh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/govuzkqlt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/giukibdwm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gaepfysjw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/grfipmnvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/ghorhdkvs.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gyohhcliq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbpwcfxyf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gvztybrqr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gghdxrhll.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gwcpuhzsm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gomvggakm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gdktqmobn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/grfkrwgxx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/giwrvcdgh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gfhgrarho.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gfqnjfuma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gxdlljetc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gihzvlleg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/guumokwxj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gslozagjf.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/giigfwtei.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gqzflsjyy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gakpsisox.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gqathqjsu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gyauggbfq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gzzoztwjs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gbjmyujbv.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/ggwljnqfs.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gerhzzcmf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzhaezyvi.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gjetaaswu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmgdbjjy.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gbjekyecp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gwinswhni.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gwljuasvz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gisnyktog.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gukdwhpym.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gjpiaqala.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gwoccktyh.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/grygjibke.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gbdaqiacg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gtsrlazbo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gmxqjnkqj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/glgxtltbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gckcwniof.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/golffumtw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gxvwsisco.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gfuvxqbik.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gaezzgjgo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ggkngjjcz.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gbxdcumon.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gbgsziftn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gbfhtclfb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gdyqycwmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gqpfactzl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgizhay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gsapjvzog.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gsplrutql.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gzuvlebhd.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gprumuydz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gwrizmzwp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwfqvfn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gavcemxeu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqjvdja.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/ghpessjjq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gocjdgzhc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gycmikqss.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gxrizhitw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gezqlnofw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gqnafibam.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjcagjr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gutzffvnd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gupnfztay.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gvwkkgfpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gondjavuh.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/guzapizef.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gjxisetxc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gbdbjukjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gofrnilra.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gksqffaqd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gaaunajke.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gliibcdxs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/guzwetuzf.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gmolgejaa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gfusivqhn.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gqzndaqvt.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gkcjcglwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gtkhsyquu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gimopmyob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gfswcsljl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gduduienn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gmpliekdt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gheunojqp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/grbomrfsg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/guhbwawgz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gfgdnshkw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/grvrazsxs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gwzjhrpep.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gseoextiv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gqsfzovlk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gtjglouvs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gwcaaauga.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gugeqbptv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gaybdqfan.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gejgnxapx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gjmdlelvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geuvdhjxk.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gniojffhd.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gexecgpcd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gnwhlydoi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghuaxdzna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gggpnjdhg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gxllczukc.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gnueotrig.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gajkgkket.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gmsiquggn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gfabfmbjt.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/grnploesf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gnrurmfjy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/giaikpqyt.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/giwnxqsnl.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/grdkspbit.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gdlagfqog.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gzgjcmbbz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gwyhfsjwg.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gaqzqdtpp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gucfkhbhu.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gsnvazbli.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gmesdterh.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gqnhtrgqq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gzvdolata.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gbotghimz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gcwqwsfjl.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gdktzdfxr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/geqcbmnum.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gpogtitus.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gzvdtxkjq.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gujatimxd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzsnfvvam.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gimpytqiz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gizbcgmsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gmmdtpcyj.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gpgxpofcb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcctuxiiz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmdjxhs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gslysfoll.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gcxoirbku.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gjdivsddp.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/glmihawct.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gclcsekln.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gwumipomr.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gqpoknvrv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gycbsnkfc.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gtbpgdcwp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gufpyjfdj.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ggflyhwkm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gsxnjnvjv.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gopddecxs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gykynrrmf.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gjxvroqwe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gmslccujj.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gdwsyadja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gxzgkzbsr.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gozqihsvy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gayeimtii.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gtsglkbjt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmqgxzkxw.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/glsavfmbi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gctwtlppo.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gpoagzwqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gquxtfszm.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/ggnqkvqxx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gecnkmpor.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/grztfpzkz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ggidrkbrq.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gcktdvbxn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmiasezwc.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gwevjwonb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjwtummhv.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gxvpmdqib.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gcddjxslt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/giqemksbg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gyejvvmin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gaikcczrw.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gjfospicb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gbplgafxj.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gurbbhlvk.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gmvkiyqdz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gknosgbsy.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gpafpwfit.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gqscjajbm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gprjowxho.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/ggzpmqyrt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gjzyppbdc.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gxexhjxsd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gopreeyyk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gbgtfyztg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gnimjmqrp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gouqahfkl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gzdfcdkdk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gjudrxzzy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gyhjovncy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gsprgncbs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/ghxjwbolu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gglinidkv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gosobyqkj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gnanuceko.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gpxbamcmv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gbmlbfadc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gazmqgtph.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grvqkcnqo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbjcmuyri.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gudyzbspn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gllrawhel.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gfnbebcof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/goboeizym.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/goitexekc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/grqrhsdcx.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ganiwmhuj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gowmxtvtk.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gyrcmjjzv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gysepncfn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnjkpoqpl.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gowtctush.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gbfhoqzur.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gjudzdzpu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gkrninstm.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/glneygdqh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gkrdvdogq.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gfpcmdjws.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ggxlhftre.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gwabjggsq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gopgwjllj.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gjoaztbkw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gzhsplgrx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcsnhim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gkxsjndsx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gwqmyyakw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gducarfkf.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gqrdfzgyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyfghkpql.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gdvcocmxk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvxlyyhuq.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gtwisewos.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gugipltow.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/galdpghgy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ghttsglvv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghjtmycuj.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/guhvyoaxp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfahhcwrq.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gailaedqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsqfpguzf.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkbtbpkxr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gdemrctue.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gdndqsdrw.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gkmbxxwpx.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/glfhkmdgd.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gspupzucf.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gfhdsuzqf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gfyqsbfvh.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gkhtkbrzx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gmfrfljsf.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gyzbkkeoi.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gtzzpugle.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gpwnwauqb.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gfkddjkhf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gvqwiyhwy.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gkyqxrtfr.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gmlxtmnxf.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gfwlfvfkq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gnltlmiui.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gvgqtvbwn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmubeceoc.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/grzspyxnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gcezpwzra.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/goaiplbxs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gdalzyysi.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gmcpkkhoc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfsycahhy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gcxoicrtb.sHtML


<!-- 参考信息 -->