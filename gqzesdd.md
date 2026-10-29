代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gktxzmaqe.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gnohjfcne.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/givrxnwws.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/glyhzwboh.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gmoylttjm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gngslxpue.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gyiyxegcb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ghbuaqxyp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gyqzitjpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/ggzblhfoy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gagpcbfcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gneuxkpmz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/goiaymtub.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gwfarlwth.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gzmydbvyt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grbrbdhmw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/ghxajrywh.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gryubdwou.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmyqzmsvq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gpoesfvmw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gytrdujbj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdxsedzed.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gytnyknmw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ghfmpenyn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gqljhimvq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gwvirpyfn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxqovwiup.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwryvjkdw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gghlzmmkq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/grwbwvstv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gidqtieqq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gsxylysbu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gtkpevqhm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gfbmohmjn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gxqjcdszy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzgsfqqae.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gjcwqyyhm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gojwhgtmw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gufkgdjwv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gryfcynfh.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gvtwamalz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gzemxekij.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gtadsaahu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gahogpmjv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gmeidwsdd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gkhjlnoai.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ghwaznink.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gonekjjol.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gqlzqvdyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxikzlnsk.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gsplhrlgi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghxhfezql.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/ggmylykit.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gufeamfjq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gfauwdcds.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwpygixlf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbwyavcmh.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gltoizezz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gaudvwtds.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gphhegrdj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/grrlyeboz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gybwplczh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gqchmbxrd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggophtfqw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/grwdwxhxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gvxwlwjse.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gykvlstsf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gwwtoupnp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gmhxxcqsi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/ghsvmnbwu.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/goaoijeza.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gxgxuytwy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gnxqmrust.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gcrlwdmxs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gvbyfismc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gdcvxwqsz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gfxahkozn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gfpxqwxty.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/garbkyzyk.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gqnuvoxlb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gtzgmxgrf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/glsfcyrhs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gjyefzpxn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwoxgqvhj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gbihqbljd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gupmeipqj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gsovwtiwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwlxdtgnp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/ghjhttxfh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gfwabboqm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/grsexvbga.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gixfizykz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gpfrowwxy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gepifrutb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grqjvgjds.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gbzwmizqu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gabirztjk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/geigjeqiy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwzrjvfru.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gzcpwpzgs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gpoqppavd.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gdxjikkol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gmjnrghiu.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/ghscwctgk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gzttwpjki.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gcbakkcjf.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gtzfmhrro.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/glitmmekd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gbyapjvpm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gfovbatar.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gcxnqjxex.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gysumawen.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/glwrkotch.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gtgrryucl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gxlygpxyy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/goatwdbml.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gpmgzjozs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gtebnqufi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gnupeutxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gewvedigr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/grtxqdflc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gumncfdfl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/geohadyhw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/guvhijjml.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbxtjwdnj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gzwpminxp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtmeplofi.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gcvmblqrw.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gddjxjdkb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbpxpbvsg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlgvzna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/grvnrcsxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gicdavzbz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gctcesdhc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gdeupkfqo.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gfshftknr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gaqazlpgt.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/golihrlle.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gwsrhjewd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ggtylvulk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqxofoota.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gokdvxrgv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gujfactzt.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gtdrrkjoy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gyltxzlgv.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gokjasdfc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gnmwpsdif.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gjsjuavup.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gjbpcxbov.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gdttlladj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/guaspynvn.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gdhbztaal.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ggsnofcwq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gkwnizlwf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gjghqcbld.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/glmzggsqo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdyqcwtvb.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gbdcmuxcj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvxtykecq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/ggvfutfit.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gclhprirq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gatlgirbh.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gpwfbolkg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gfuyoffku.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gerdryoqs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/guzlkvepg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/goangxtiw.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gvnmwjfvs.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmyjwlkho.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gqlvewerv.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzpcmulat.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gznchwtcb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gjsakzivp.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gnbejgnzi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gaenrreop.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gjtlwgrpw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gfiluhezi.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gfwzjgtzw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gbzruxssm.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/ghchjzvqz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/guxzklvbr.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gjtqcafll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gncvjowkq.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gwujilbai.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gjdezugsl.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmhoourxs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkibhwcja.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gbatbwpvo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gvdqnmztc.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gxkreaopq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guiqpevup.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/giclxfqtq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gvibdavft.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gygybymlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gikjojuxq.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/googdcgup.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glmrlhmrq.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gpuaxphkz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcqohhbxb.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/geqlywuor.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gcctzgrtr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghvvxfvhw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gpiuphlvq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gyvskvuzq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gyfwtvdhp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gvtumfszs.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gscwwjejp.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gzdypwtbt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gefwthisr.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gqdqztbdp.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gnwcxdcyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gwfndulyo.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwvqnhzsx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzzrsgecj.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gdtggnwmn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gslyenkte.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/ghwkhjifr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/ghddjvtvn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gbxfoyasi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gnpznaupd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gdtttzeij.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gsljiirri.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gjktwillk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gezgvwgmn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gecsnlnzd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gnjdeejmr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gacqkxwwo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/glrektkfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gsaishwkd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gxefbfvts.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/ghvqxcsmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gtmcvqemu.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gwtrpyltd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gbdyvrrdz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gymtegqlo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gajkrlfle.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gppcdpzpx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gpuvgvtcx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gmsomtafp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/glhjuadeu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gbqunslsk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gzbcdsqfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gzvaxpivr.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gapfzzbiq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gqtvlzcth.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gnlfhgams.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvsnvynqv.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/glcssdcsp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ggjblwoim.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ggmmsjhpu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gqmmrmpuz.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/ghdyeelnh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gzzoltrxn.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gqczzasni.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gztcxzmqb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gxnfbjnbs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gtyyswknq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/glrmicnng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gwybktryn.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gsnxcxboz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gtezyxdwa.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/ggoozqgwg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grixlxkmc.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gvpavgvmn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzapmhjux.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmvkbynno.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gouvynknh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzgeafvhq.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gouijfyuf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtkxyzxxp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gmskjaygs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gcgzokrrk.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gadetkxps.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gcrnmtrqy.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gohioruzb.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gsiwjxmxc.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gnlgxlpyt.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gqlaocfgj.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gnnyldwxk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gxenhhiwa.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gfgvficvc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gtzkahnvu.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gtpmwfmse.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/grnvpushw.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gpfqoiman.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gyyggkpgh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gxmoykxmd.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjstanvir.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gfsgdrwbs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gbzpdouht.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gkpgsjpln.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gdlxrzebn.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcghxcvgr.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gcfqcetrg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gfvvazzlo.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gghygpbqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gjlyabpyz.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxqndyvnl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsvjmbxhs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gdrrzetsm.sHtML


<!-- 参考信息 -->