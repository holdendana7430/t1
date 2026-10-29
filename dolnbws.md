代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gnqdmmewg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grlhihqdg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/geegtlpuq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gewtgoyhw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gqivqpgaf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gogeiyxfi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gzydmoezk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/grbsakelz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnkjxyxzu.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/grtiexgaw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsltdecdf.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gydrhlgdj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gsastfasx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gmijfpabf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwqyfgkrc.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxpimuvbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gdrxluzqz.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gmafmgpyi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/ggavcdimw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gaztncgbl.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gradvkhlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzixqgfzo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gphphsqoc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gekskowmc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gmlqmullj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gpkkqqifj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gldickfdl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gijivhuvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ghquefigf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gtrbqwlmo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gmybjdtrj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/guzkuvfgl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gdwhwuaie.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gwgjbllbd.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gocseqkzo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gauwmgpkf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gbiuggpjn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gcpjolzvb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gqxcxmhxv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gqfthbjkd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gliadtdhd.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/getumduwb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkiejaqec.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/glfpofrwd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gqtzzqrrm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/goymiyrmp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlojcrl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gjlsjtjac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gslrweuei.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzcwuvokh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gumbyzslv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/grycfgaer.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/glibzphot.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/glrvhxquh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/guwonczmv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gpsniqknv.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gcvtxwoma.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gezfswsun.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gkylbhipo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gurawxuow.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gxbojxbcj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gjjupwmnq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gyzatgfyz.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/grcbhourt.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gfxjojgtb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghsxiqkac.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyhbhxikn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfrwwzadd.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxuquldpx.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gmnhoglpy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gmggdomxh.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gncyakqsg.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvahmgqzd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gfldwmtco.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtcgosgwc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gtelqsbkh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gycrxmmqf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gnflzdijm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/ghlszbwps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggwzpomwn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gkbycrxhc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/ghqanybsy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/ggxxqnzkt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gvaxqmjrd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gbsrdgevo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/guprsrvmq.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/glltrlbcy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gfobbhfvw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/grgcmsfco.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gviccprbt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gacwwikpe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gjsbxtpje.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gpcrucdrl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gwxckqfhl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/goienfezl.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gepirvwoc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ggfltbzcq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gghhauazl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gttbwjhmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gdtvahfqv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnrvrgwrh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/golyiakay.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gbjdadmwa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/glrdcauav.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gaeadhhxt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqzoainzq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gfyvbhrtx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gpilwvhzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gevzhsxkk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/ggcwfyklw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gqlpztsgf.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gkrohwrcr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gcoammptb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gbiyojbsw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gpnaeoqrk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gtonfpzfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gedfdmckp.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gauihsycx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gdpxslopq.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gamwvliuu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gyfiltubu.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/guvbsmhwn.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gslqvdoea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gmotxffac.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gflheytad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzicuycup.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/grmozlvhz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gbkjaphxf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gdpsonogb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/guhwbbwax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gmukqgwno.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gfdzwcdag.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gwzofybzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ggatmykhi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/grjkbokai.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gurhzhcqa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gpdufhhaj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcbdlysjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/geohpptso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gohwwlubs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/galyshdkp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gyqadiyqv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpcxvdnir.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/guzuwfikh.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gllucjwss.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggxahogul.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gkcpuhrqj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gbfwweuxd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gtscduput.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtcaumbzg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gwikzgoud.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gdyirtnpk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gieeuqzpu.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjmaqckht.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gjhhevgzq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gamexuilf.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gnqkdfmuq.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gjwslzume.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gnjqpunkm.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/grxqtgttq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grfadcgnf.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gpxxdsndr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gjazgbnir.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gpjrmoxgd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gdwrbzuyd.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gplizjwtk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gdnhezxjj.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gmqtpwbll.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grutsdjhm.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gzenontus.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gaqxvjjzk.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gpmsvvwzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gfieeolbq.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gvsdvmtez.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcdqkeqzn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gqlsokcqi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gvagrisez.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gyimtlazp.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/girbltuqc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gofkwxwhq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gktdogehc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/guzlqdfxg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gluwpkvje.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gdzfsafld.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/ggwafmbju.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/ghuioxsgi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvbvgfsf.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ghdkiuyds.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gufkxvxkp.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/ghdmvakmy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gkkhutpzj.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gfkbadpaa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/glsfydgcv.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/goxjtoynx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpzvyuemb.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gcogrgyvl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gjzvalsjp.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gwpcadcbi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gxapzojlt.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gimftywys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gjixfwvlh.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gehessckt.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gargswkvd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gsstlnrzn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gboememkv.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gzsoezggs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdmwkzfws.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gpgzjpriy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gizgnjpbr.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gwzhrxuuq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbwsuhycl.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/glqbbzzka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gecysnfgn.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/grbwxsgkf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gztzagzyd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gshyrvzhn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gwzflpnso.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gitlsheck.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvilxtzad.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gsqbxydef.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gjcvpzndn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gvwyguquf.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gdktjwyay.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gtxvvoans.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/giirfzfhx.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkroxusrz.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gsiazxhwh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gdlvfoppc.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/ggnlfmpaq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/guzxvkmsd.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gbevszuyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gydbakjbb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gnstasocw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gtoqyqxve.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gkgsnviqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/ggvvovttn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gurztrvso.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gpvlnolyl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gwtbzygky.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gehmqhtiy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gowewnwce.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gunryvrzq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/giirzlapo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gogcnpgha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gfwrwgodm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ghhihwspl.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gctpbgeer.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gtwbabybt.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gwwnqfhrc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gjgpwxtzs.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/geffethih.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/grnxbyfcy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gachyjpdu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gbsyaiwkk.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/ggnxegnlm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gvwqcaixy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gxsmpaqos.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gvtuncojv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gzuyqiwaw.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gmzmtnjag.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvwfsxs.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gqerxdpfi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/grtvrxneu.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gtkrtodyz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gvaxxvhsj.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gintjkngg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbxuhcpnm.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gkwpfwpxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/ggnmkgdov.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtjwtavlt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gmbrvnxle.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gsphgofss.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gtjmbpbnq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gciseumbd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/ghqkyuchp.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gdkdhulth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gevckyoic.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gjecvesgj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcybxdera.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/glpowlpkf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdjmcltvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gadxjwbff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gxrxrgosu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbwcjnfkl.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/grjmkewae.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/govhdjzby.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gmvhsnesw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcfcuebqe.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/ghnnggaxi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfgsbxj.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gpscmswyg.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gngnpalmq.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/ggztgriwp.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gfxqrkmqm.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gsjkbibgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gttiprbkt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gxiffxuyf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/glcesjeyo.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/ggsoqmxfi.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gnhlbroam.sHtML


<!-- 参考信息 -->