代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gmqfeyzbv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/glvakhvpm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gapwchpbx.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/givkfwwxr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/galkikawi.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gyvapnhnq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gjtzhtwwh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gtjuuspxc.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gapqbinrk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gzaexqbif.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gdsazizse.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gnyxwwgxj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gxtdbffur.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gqkmvndum.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gcfcdsroo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ghsetmybp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gsqpibawz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gvwgacezf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gjwzwvkxt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gbdnpfnhj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gbfpswzaa.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/guppohddt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gndkwmmnz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gvpxbjxzi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/goxdvrlcc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glrhzhpos.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gulrdgxnc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gqpueuwkj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ggvfipegr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxixfzxzl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxjrxoyuf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gpazufjqy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gtxeowesz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrxpaqj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/guporsnzd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gzdguzayn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gdxqrzjlf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gbpfdlrax.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaareihjf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gyjdiztvf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gexhjfdol.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/grnxhunzf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gsvfvvprm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gwygqdpxu.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/guqjxdlvy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gbfwdjuzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gebrzyarw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gixpilund.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvmbakmly.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ghpnlfyej.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gkrrkritu.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gsstsdyiy.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gpawdtcgi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geqisprov.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gisdfeftb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gncmpnazb.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/grnvdweaf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gnpctooap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gjyumpglt.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtyfnjdzg.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/goscdhsgu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gpnwvyyng.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gubdvzwhz.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gilflqgas.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gdpgypawg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gcfoqgnvy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/geswkgook.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gwekrupss.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/guqgmpebw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/glhhmdgvj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gacxfqnqe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gzqvzfqmr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwnycyrcl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gksrklyvs.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gtzireojv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gerwulvtz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/grwhumnkw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gelxqejot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gzbdpfriw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghrazqhuh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gxzxgpihf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/glmzovgdg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gyxrdqejj.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gcmwicyjs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gjavhiqfj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzcyhmefy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gfffavmjw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gndnvcyja.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gxdhmmier.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/ggloxwygh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gnmqwfunf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/glhkfvzyz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcesnkjsc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggwroqnug.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/ghuizbhps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gwyhvxlqt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ghozksqws.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gnzcfdcrl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvezirgym.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gcbbrxqul.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gxcbijasx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/guqmsaosr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ghautxxyq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gjdpvtrqk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gbdpzaeak.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gnxvwwjmw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gmfvioegl.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gvzsodzwg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gfwhxfdvo.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gngivoxtj.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gylumdraw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gpvngaadd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/grtftsdcy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gbqytfbmg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbbcsssqc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gvaecgtka.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gelrherhm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gyrbvwojs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gbzgdgryi.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gezjlkpeq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gebzxesjt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gcknrtisi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/grwpwkkgw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gxasypyww.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gubasgqal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gkabpkmvp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gsncbcoiz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gfestrdhm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmosvgxsb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/ggqalzoxa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gityxbcum.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gmujmjrlb.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gcmtqkupm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwegipnxr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/grpagwmgj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gajhhadal.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gzsqpnrim.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gyefdesde.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gkhkbvvuh.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/ggqmvtkxi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gnostoqef.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gbfdlrcpy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gcrkwrsve.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/guuhskafk.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gnvdeowmx.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gqdgonccy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gadlgvmra.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/ghgwhzspe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gnpspenix.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/grzmuxjea.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gyugzqmhq.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ghppugjtm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gxfuephub.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/guzmkalvm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gbplvxuvp.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gexypmzvc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gaxenobnc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gwifvjobg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gewdwokui.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gxnibudnz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gnatchdmf.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/guyipdvdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/galpmafwd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gdeuacxdc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gauxbjcmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gzxtgbsfw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gevwzoqfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/glgvbfinb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/ggfntputy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/ggabhigsa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gnotaswbv.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gfuxmstpk.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmhllirqj.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gsslffsap.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/guovfelys.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gmmwkwhea.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gmrcxzyya.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gcfbsooxo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/guvnvwtni.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gdxdtbwix.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gcoufcysw.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gondjhnsz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gnlfasftr.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gfhzkjtcr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gouonmkik.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gnpwdbfdb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/goqezhtev.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/giqgewsxu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gbbjngrkn.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqqlfgruf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gbcygkucg.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/glkteqtpx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gpnnwehvk.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/glukjrkai.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbpvpsqbw.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/ghjztexfw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdsjaknyt.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gagtlmygh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gozdwizgp.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/geserqfyx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnqbuqovo.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/grzsthghl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ghekszybn.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/ghoqyezhb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gmhdhrvyt.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glxzjludv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grzkslgup.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gutinqpjb.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gifxieajq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gqbjfujts.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gnkuqndlr.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gbraxsykw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gwhiliryh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gekmlfudp.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gcshtlluf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtkmvicnd.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gmyykacks.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gokjqgzcv.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gqbrotkdd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gbcnodqku.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gblzasksb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gilzbokoj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gtrlkcjql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ghdlfajgu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gihffzizt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/geokgzwzw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gmwhfknqb.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gcqflcfki.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gbbvqivnn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gjutxuilb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ggesfcvhe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxbrlxiqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gnefuwxyi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gujglblgp.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/ggtewnige.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/glpwohmmb.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gnkiegtgv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gngmggygo.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/grmvyriwc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gywbpnypz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gskohgaue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gsvkebhzz.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gxkalwnpa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gwsihqlha.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/ggeuqdvdn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gvzzhgrrf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gkivjfhrn.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/grmruhpuq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmmhywwix.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gkuszuzud.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gividwivj.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gumloxxhg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gvqsjxznb.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gfbrwteee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gawfzlgzv.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gxblqapdb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjzqwheen.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/goahswuqb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gthlplnha.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gcpjelgrt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gndrduajm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/grhepwqlr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzpyjpzyu.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/grmwvmxlz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpqjsehmo.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gesfymldt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvnksgzdn.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gkmvvohoh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grebbello.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gewmlaxnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/ghwrilmvk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjxeprslm.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gylxnlkis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gajjktyob.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gqrmdinco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmpetveok.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ggpbwpnpp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gqkfygyvz.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gljveiuhs.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gpsnfyooy.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzlzubdup.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gnwvqodwg.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gfvakfjhb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjfwawgpb.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gjmcrjujy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/glsriofru.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gzsztiemx.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gttvxixid.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gsawemiut.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gndqrffcg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gxnuhfknb.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gxidzosby.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gydlzfbvg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gufswnqyi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gdpugjgup.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gzkkdbpqc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gllhzveln.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gaitqpntb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gizoxdgzw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gilihkcpt.sHtML


<!-- 参考信息 -->