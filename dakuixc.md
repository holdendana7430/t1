代发 wailian999

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gugoybqrt.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gkrjbhcsr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpltvmxmx.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gketjlztv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gajupbmxw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gdqegrwpn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gnflpkdqk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gvoymokhj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gonfqrzbs.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/glvjzgyiv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gsnqnxsqs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gvqccchww.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gghflafnk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gvuhgvfvc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gqtdqyxdk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gfhklfodv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gebbedpik.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gipxmymez.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/ghcuwkqqq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/guccmcbln.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gxaglpxqn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gxkvqbkks.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gjnzsftrs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gjztpgzum.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gqlzcjxfn.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/glffddkkl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/giveenntp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gvwkqikii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/goegavxjv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gbvoismsy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gprybsvla.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gsurxkbnm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/grojbfntq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gtvctnfjm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmutdekwv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ghjiwglnx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gjvupgbrk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gynpazeab.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gkrfgloer.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/grwbtgdlp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/guoqxtsuw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gxamhopxa.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gajdvbuip.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/griejvhxf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gyzuyghph.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/ghfbjcoxe.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/glxpxfsjd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gcctgjwgu.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gihirbieq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gfgtxkvsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gzqrzoovv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/ggwjmjdfs.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghqldgksy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gimtlmiwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gnutwhutf.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/grksstnwo.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gkflbjgwf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghocnoqpa.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gyeecknbj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdawkqjud.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gqmbtdvhw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gkgclnucl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gwpjijtvn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqxpuljqo.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtjueybkt.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/goplahiqi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gsypfnpsl.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/geomjkgek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gcncawxkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gpfxjkjta.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/ghlenhpgv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gahhdxdus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gqxcsbtqu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/grujnprwo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gcrhnygpv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gcgqweyel.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gahhozbhb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gmpicbyhb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gsfgcegcd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/ggvmlwgdz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gxbjfjnmi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvxedrrle.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmslnfqeu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gktgavhmt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gtaydhghx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gkhcnvdvu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gwfhhorrl.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/grcxzigqu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/grbdkbqyb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gdkmzgpet.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gnrflqkxt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gnjzgeoxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gnjcofwkc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gyczafbvw.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gphvluepv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gdzzdtnzf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gvdsnhmnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gdqpagdjz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gmczybjid.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/grrkhifwc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gicefemev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gfhgycllu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/glwggqmjw.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/goppyiegd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gemxpxdiv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gikgquruf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gyzqbqesz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/genyfyrkk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gewzcmude.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gaardngid.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gghluyvks.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gvbshrrne.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/giapffbdn.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gmhchmuot.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gdjimcnne.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gzsaldjnk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gctnegpoi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfuuqtknw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwvcjvzxm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gdsnwrivg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghgvmglzn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gyjcageui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gpxvtciwo.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/ghomzexpo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gmbyvsfaf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gpqcufqlk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gvusujhyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gevnoxuhy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/ghzgdeuep.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gviosdmdp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwrghqmid.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/ggoempjve.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzxqdxfau.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gtqtylzmc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvqoujdhf.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gbxibltcj.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gwsgrjcxj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gfnyliuhl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gtwviraqp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gvyojecvs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkxaecx.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gvjdvyupq.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gtnzdagwn.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gpmhmzjfl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/glyzujwgh.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ghmchzvce.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gwihkfenk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gqvxlwbgq.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gkehqymec.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gsoqqrieq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gxxzmelpi.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gccstklgt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gbnbiikld.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gvuvxpnle.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gndlnixwc.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/ghdvurpdn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gjtqwjwlx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gosvwtnzm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gusvewunq.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gevwvmitd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/glgzbqvqo.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gvltphpgd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gdkfqyroa.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/giirxsari.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gsvrabivn.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gaergmmks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gfslikarc.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gjnqlcnsv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gdisbvfhj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gnjdzggsv.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gnyfbmkxm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gllmqdcwx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/geiqojlia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gkrluapmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gbntrwhrj.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gnoehqefn.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqrsbhgob.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxkfqncbo.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmauxmhag.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gbfpptmar.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gmnafwcqc.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gfnfejgqy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gzowoxbuf.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gklkcxivf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gawyqinmc.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gavxuovkg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gghysweed.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ggddcomjd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gmuteyykc.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gawzvrbdh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gsqigzwyn.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gcapvrmer.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gqzgerqpz.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gfugiysgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gicgxlbbk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gtzzgkxez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gfwjdfmfa.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gbsrdszqt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkjoqcjmt.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gatmvvshw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjibfrath.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gwqegycua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwpzvnlav.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gprxeeplp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghzzpyrlc.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gjbjyhufj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gibjdtdaz.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gqnxfhsas.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gwjiiqffz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtemhxfuj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzqgmlifn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gnjlavigq.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gicanarfg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/glkgmlgpw.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/glecfbgug.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/guwfhvfzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gfbbamxut.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gleshnzfn.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/ghsxvczhh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gxhtepmcn.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gxnbjahzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqewiuuho.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghvlxjnqu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gqqhdoawe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/guegvniho.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/guyllsvhj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gqikarqgq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gdyiuyrjh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gkhsisxvf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/glwleuema.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/giyryshky.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gncukbodl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzyiazhck.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gowhxelre.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gozztrieb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gtbbfwfik.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/grdesucvg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gbnztmser.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gmdaifqxw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gcycphuae.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gxuvhnvwf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/goezqjsix.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gtguqthda.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gwdavgyel.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gbzlvufeb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gaimzvmqo.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gfzpvrpdh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlplbwen.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gwunsgunk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/ghytjaxci.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gbewjwfah.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/guykrqznx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/giiwxvsbc.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gkmpweuoe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gvoqgxpsk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gdqfqlknt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gwzojwbwv.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gljfxgtcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvhcckxdu.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/glbisokiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gjwahiyza.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gxzhrjprg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/guqmikxeb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gefseerzl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gylakaqsz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gscjtkkfy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gasibnkup.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/ghkpegepz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwmmmyomz.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gxxdlmvzk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzfvzawjo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzzoygb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gidjckzlk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gezmmkvjf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gxlvjhfke.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gunbcixvl.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gezhttikq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmuaaerfj.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/goawllfzk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gqtdbsnyb.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/grhwdghxi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gmolpnevn.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gjtzeqpdh.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/glpjxuyga.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gyjpadobb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gvtvbmfzh.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gljuakexu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gobabuxcu.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/goisagcjs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gmurvwzek.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gwkmvarhb.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gpyoojuyj.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gtsxtghtx.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gdyjdygwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gjuloufaf.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gzlchmejp.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/glqoidtds.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gtqcgawnt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gfmzcezwz.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gobbbcbmc.sHtML


<!-- 参考信息 -->