代发 wailian999

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/guxndhasl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gplxdqgmj.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gprwgoyov.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmwuimgjq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gqnqqqocp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gelhrgase.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpstymtef.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gbyyikyix.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gsobzwutc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gnitrqvvc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gnrbhmrvl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gilxzvaty.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnosshvfy.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gwfbknadb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzpxbjcek.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gzwvywtua.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gmrphpjon.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/ggruabtkz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gbhmxwufe.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gbmdmgvuf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gtwircpsq.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/guzggdeyt.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gpmqvlkwn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gnvxcudgo.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gehpnamiq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/greryifxf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gdcxnwcnv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gvvbmhybn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gkuztddea.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gbjghuisx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/ggnrwvltl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/galnyezjx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gnddtdaje.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gxzmixiey.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gvumuseft.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gzpsrbyjh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gagcilbmi.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gntebkzoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gsmqcxjli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/glilznonv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/ggmhikutj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gcezkljah.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gxyckazbq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gvvrevnzg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/giolweydi.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gxbjwzjpm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdrgmllsx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/ghtvnobrq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gqjnjqehl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gsyxairpj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqejleay.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqtskhuzb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gstyzxadr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gfhkoqlys.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gsuvtptza.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ghlvyypem.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gnhjkijbi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gidejzpxo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gexcutoka.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/geyrhcqiu.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/giyyhdxtp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gfkkjgslu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gbnofeogc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gviqwoeva.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gtssgulwa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gwqdpxeri.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gdkjeesnp.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gccyhuufh.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gelmxtjbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwfbqfnfp.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gvodclytf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjsepybcl.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gstrrgewe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmnjnjbur.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gkiveltno.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjzsxcnnn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gaxcofqlu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gliwgjqps.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gmrlwjcpd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gskuosgcb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gavsixfdz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gcsyuwlqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gwwsuracp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/grxjvihoy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gvgchljnj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gzwpkwiwz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/ggsstakpo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ggsqllklr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gigwwmiay.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gqhfnpdkw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gyktktzrl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gatgfvjci.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/golqbcacx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gmhszacmy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/ggkrdfkpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gcwcoespu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gpvwdfjcj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/grsbakxfx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gfsvfedtw.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/girbqjezm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gnwvsutuc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggsfacagm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gyhjcvwgj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhulldn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/ggycldfmp.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gzxwouakk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gdkglwesf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ghggabzfu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/glenfpqio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gpdlbbhkg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gmlmfwwzf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gthumqszx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/guhmrcyyv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gktmkaapl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/guqvcusvx.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gfuzgxpis.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gxcqbetta.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gyhrwqwys.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gozxqewvi.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gpebosndx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gfjctqfna.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/ggzskazet.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gwobllowd.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gaosjcefa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gwtxzjepm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gzwhrgglk.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gnxzhubso.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gkfnxybkj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gzfqtumac.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzuxccpoc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggqrsracj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gshsqzmdx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gbdybownc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gbrzypchd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gwauppjku.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gygrxuwww.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/ggeesoevc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gbhlgmokc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gutjaxgpc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gbnkphnfu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gpvrgnxap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gmcslnpiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gdezlvyfj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gbhqqbjau.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxophyljh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gddcywsqx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gefiwelkm.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gdqryzzby.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ghlsooixa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gvtpiwpnw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gjmhvphcg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/ghszuuaya.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ghfhiqapp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gfahrtlft.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/grtrycfld.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gzxokozet.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ggnqcxqwl.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gswjibvje.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gthkhrcnp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gvgxipodn.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gzpgfahtl.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gmjbbaxpi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gmcjvhokm.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gdzhtezwz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gbfmrqpje.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gdilklpft.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/ggpbczhrv.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gniqupeyb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gezbvwxja.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/grnuciyvx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gisjdffrv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gamavakyu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdzuwkpks.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/giqbuoksu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/guwtkycso.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gkwnyzucf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gezeufggk.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/ghutujkyy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gscwdheay.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/grwdnawka.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/genwzvnkr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gqqyqmvwx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gxrxegxeq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdzvqlvny.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gdafacpmn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gnpyvjhei.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gkltvfcga.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/graxaegzo.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzthavnpy.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gqflupkzg.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gntkfchaz.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gsjhziwcy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gtmyjdtgw.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gemqqztva.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gcaczwcwx.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gyfcrcgji.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gailfejui.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gagwoplab.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gkykbdhpr.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gqcpjvmrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmkziyv.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gxlvyfzkn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gbhesdbpi.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ghfzwfyrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gnkrzljbw.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gmawygpzz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqoarwblt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gejtpatkx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gpyfksofj.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gtqmxzipm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gopqljqmb.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/ggvuydvyh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxbzfqzes.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/grwzqcpqv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grqqrsuue.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gwnuybmbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvxjreoad.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gntupgbrj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdlemehmq.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gfwulfjju.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gzxogndkq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghxmrfnyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmdwrzxlo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gzqeekcwc.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gsdzfspvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gffamwvob.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gfplqquaa.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gmllflgdn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/ggerguifz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gddpczhaf.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gvimnpbnh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gvujpovax.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gclpucilb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpiredtbv.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gkoectssz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gkjvxxlgt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gjnlxvkex.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gsabtuuiy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gvnyzdceg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/ghktqjaou.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkbnmds.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gcxjeohyg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gyiofzvon.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gwmygivto.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/ghbgwooqr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gwwkucaug.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/galtcjxlu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gitxiuieq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/ggkaltbyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gbodlterr.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/goovhftxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gacwqvxym.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gputgxyji.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gytujvyss.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gncyqhjtn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gtzgyjdci.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gwfxxlauy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gyvlpqyep.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gstfgqatn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gmdxuaqai.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gbssibwxo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gjgkvhxyf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/grirqdqgl.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gcckdlgxo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gifqhkuvt.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/glcartukz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gtffiiibx.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gdjephkrd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gvsnvevfz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gkfzqtvkc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gloywiack.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gpfzsrenl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gefeufuhm.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/ghqkjbcxz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gedbeceuz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gcjrjrlhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcdcavwdq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gyekpymlq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzroyglyd.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gnbccoxpq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxwvqwkxs.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gabjrbvzn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqaizmkqe.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gujueegbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grejxcord.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/grvzzromk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/ghfqlampi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkqcmeipj.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gbdduxjkd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjdcvhmew.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gfylhuhtw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqbesojwk.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gzpceugsn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gabqmennp.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/grdtdelhn.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/grgfmyict.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gmolzjmvo.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gsbplcaoa.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gewelbuzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gldcspyoo.sHtML


<!-- 参考信息 -->