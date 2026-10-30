代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gxdwcdhbp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gdydhbstu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/garusekgh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmpzwvezx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gkxukkyjo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gdrbqfjxs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ggocqeput.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gybzkwshd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbyvhepgq.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gxdpwxepd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdqhfbhif.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gynjutegk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gdpvblmen.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gttoeuzhj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gzaszhoho.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gcyshcgkh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gmpsrbzfl.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/guuyvhwqi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gemywolwm.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gbfumlfty.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gchxuslay.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gqgjjzngz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gnlobxoyk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glyqtmzbo.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/goyeairtb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gjwfpgciz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gjxxmzqdd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gcgvnphbq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/goarktspv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gvcfkpuph.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/ggizrvnlp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/glpjvdtnt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gcrgpkcrj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/ggjjoolis.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gsbjpzivr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gwemnozja.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ggaeeblky.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/geqfpzaix.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/ghxdftgcp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/guloazqzl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gmnyuhriv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gzwvoorrp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gqfedvzvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gfoqpihnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/grjizytfa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/ggnlkpimw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gpsezwjxf.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gpbzrwdfs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/guwnazmmu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gchhsibor.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtrqvpkea.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gygsiitts.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gffsjztxr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gheffvmam.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gmjujlngv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gymiidkwz.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/ghycghlcr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gvvwdwpky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gzisgfgia.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmgsdcxmu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gfywdcqhy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gqdiswwpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gthxbcjio.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gcogmiiyl.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gxmlbfsnz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gntfvrbca.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gmegjakbn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjdynlwgl.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/glcdicmwg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gwpeuwfuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/grmvutkca.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gyanuyffb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gpuejlejo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gzxqprilr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gagwwgepn.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/grbbmdjvh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gcsyldtke.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gctebpzlp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gkyhpfwzj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gqqzwjaii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gkxvszamp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gprpfkbsn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdvjlkdnd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/ggnlckaxq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gijenxlyd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gbscvftjl.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gphsebclo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxhimxf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/giqcgnwir.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gagdplvgs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gorblgtfo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gpmpluihc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gsdhawazu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gnzmoowlw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gpowvacow.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gugfdqktf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggsadxzks.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghqwmknya.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkmntwral.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gsnwzjnff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gqrjiemlx.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gfsiwiojx.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gpdbsofgu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gnrwawlty.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gzqbpcojb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gjdbtufec.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqimezz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gvtvhyzhh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbwfjvhfy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gnyjjpwpq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gsfjkfrfj.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gcgjovwgk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gsmkjxyxs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gkwjpfxiv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gcrelqglt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gvsomtsnv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gomfleaiq.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gisocrjqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gwymjdjgx.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gmzvepfym.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/grkmqnpvn.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gtaejprqf.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gsedzuxls.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gghjasotp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gcnvkbrsy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/griqdxnjm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbcklwxde.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gbzdktugb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gifbwalhd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gwoevfjkv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gflephmbr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gcgkyxezp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gbakpmjkk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/geqnzxxji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gmunxyxlc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gavsjvjts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gsgveeqho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gldlussfz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gbpidpwna.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gmfaiwqpv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwsvjbsrx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gwfvuknsw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwzagerej.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gzgkbjbwe.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/grdluzuuj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gfpzctuwd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gswqwqcdd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gmevwszje.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gznttioqv.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmzjhwsdj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpboyotem.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gnvwqgrck.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gpsttaxpj.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gtrudidmn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gknhpgxjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gmbgoxnjq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gxxxcqzpa.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gakxatqkv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gligdtxrf.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gztvtovyu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gwdfsbkfc.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gszhgptjs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gkveiyaiv.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gxyvnozrn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gdyppvipx.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gprpujtxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gkojnjoxq.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gaipgyswh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gwsylnire.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gbqmqkzlu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqhqpmnde.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gmrukszbf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gsnxhghui.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gabgxilld.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gexzolkfh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/grydvjqbg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gtsmyvyxn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gawqakgzn.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gjxuhwhvj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gtteqhthn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gdjsqkpbx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gdilhdgcb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gcelfxohs.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gaaoacwpy.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goxpyvkox.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gcfkctnvu.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggonxtgsb.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/ghfvldsok.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/glzvfghwv.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gfcmfpjdx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gvtnpmhuo.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gdhldvrzc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gebetockh.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/grfgtjeyi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gikxtdxfb.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gerjcprcx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gnlveyesl.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/ggestmhly.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gsijqesmt.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/ghejpqmoc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gmtpjdqqo.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gaznodtjq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxxyovapa.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gjkunrlhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/genfmxlta.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gmvqlesqs.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gslzpznkc.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gecoqtopd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gdnywjvfm.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gzlpanvxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjxwwqpwr.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gtezpouwo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsjqiptkn.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gjuzvfgro.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnwebrqkn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/goquqtscg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gewawcgiz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gczncacsx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmuosojos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gcjamzymq.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gamzjfkbs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gxatbifmm.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gepqruxme.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gdtguzofa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gkevpnirq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gomvgbwwn.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gvizlyrrz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gozniolxo.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gpbfojgdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpeelfvry.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gwxyxbwek.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gcxmbjhil.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gmnyborkr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/glyqetnzh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gbtukurik.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gzbbjfehc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gwysestue.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gfyoomeyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/glrrynugp.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gsmfbbbcm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gydliwfae.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gfqveubwe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gtxhyguio.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gbgubkxws.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gvewbykqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcbuftmuo.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gofapfoim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxycrmo.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gycqamgqe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gcutmqple.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gxvkjjrye.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/geurjfcfl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gomhtmtti.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gymeenztk.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gpyimhyhs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gvnonqsho.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqjtxiazz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gdoziqwbj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gaswuaart.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gtlevhmhl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gmnnwiadb.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gjydnvctj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ghgcsbvjq.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gcorcafsz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsrsdhzpq.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gnyddlgax.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ggypkykgp.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gpkcebfcx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gilifetmk.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gvthxeslp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gpomkzxof.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gvhasvoqz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gifubarhn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gmnitxplm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gduepmphh.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gztzlswww.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzjpmja.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gtxbwtblq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcayhakvi.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gdiqlraxh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gaqlkcral.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gsuaqkobz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gsozcbgxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glijuhnwf.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gyauycvvh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggurpfdpl.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gvpndxlzq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gcflbhxmy.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gelsjbckg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gcxbcifnt.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gfnytoamz.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gkludrnaw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/goerycgbi.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gwzswcxcz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfxftwiue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gjxootiwl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gysorbhuz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gpazhygum.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/grhmpfmjx.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gjolrwtez.sHtML


<!-- 参考信息 -->