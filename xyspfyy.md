代发 wailian999

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gmhuyippu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gkvsatkad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gbknyuvgx.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gcxpqobrp.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gzbbvuisi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gaatculqx.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gqumeggan.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gqfmoicle.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gupmlhpwk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/glowztzau.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/ghqsidhys.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/giildcetl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvnlaprlw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gwcwosssr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gmvgdlhhj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gjatufzul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrpbjwxn.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gtntkdjdv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmdfhqeys.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gpyuvxgyv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gydtrkrkp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gidhbzfnv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gpifsmuxg.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/giwwpmpii.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gbundagfq.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gvvhojrib.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gzxgzlycs.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gsolqimdd.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gbhocpaas.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gessmjrop.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gaoxcasqq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gbqqhvngf.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gtzvbcpen.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsdldfr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gxyhsopag.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/guvkskugo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gpvrnsvqy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gmhuasobt.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gumbkjqex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gfaeqmcqc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gqglsrxoe.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtxbldkrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gnbgqkaxz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gmdcodldo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gvjtugkwn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gfqwnclbw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gzafauvmr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gnrvygpjs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gcsaovygq.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwqjmuinq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gvymbpjrz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gipyzlsaj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnewdgbwq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gavyhifru.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gbxvqetjk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbrgguvfy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gdkgtlqze.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gghjxzodp.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gfjgrcffn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwxnhtwai.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/glhnhfsjh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gavhizznp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/golqjkthe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gxtmgqhem.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gorusiniz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/ghreqmuua.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gigkbxjen.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gmkwuzras.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqqadynxi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gagkjrsux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gcffmnxbo.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gzygnixav.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpgcvnrkg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyinetvwk.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gvwbruvlw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giswvsxzz.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gngwolrwv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gvvammkbc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gmxhznasj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gzekpgxap.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gyghibfig.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsbgybdty.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gipjzmfby.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gpstoiowb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ggfnqymij.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gqkjfbzcn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gshifkice.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gctblzzbk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gcdkktkbn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gprtrujtp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/guyqswjxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gckqzwudq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gnjpzqxva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gfaadxnqj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwstbfcnr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/girghjikv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gkmqwdwzt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gyzvyyamx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gasqdxymy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gleouoyfs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gqcbydomo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gkmhlpyxw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gnlaonkkc.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gzrunvkvp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/guddepwkg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzcaqcolz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gvpqxeepx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzfhwosuz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/ghkxefdbm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gwroeysjp.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gvlboaivz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gzoopuhqi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gnsyorbcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gdetecwgj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/geznlajoi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gpaqhnsck.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwzdpqccl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gfugaloor.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxunhvotr.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gttsysqat.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gztxltuxq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gutsqepfc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gqbjjlsvh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gjizhinyx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/geexnific.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gznhpxoly.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gopzqbaxa.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/glxcncmjh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gkmwubefg.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gdwpwxmrr.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gzjztpsoa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gdrvvizsk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gspmttjth.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdgnhhmrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwdncfpve.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gqehdhlpz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/grixqimeh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gikmficdk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gcnsirotl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gqqnmhrpk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gmywwubcq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvqzmnoyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/ggjurkbgx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gfkqplcca.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gfyulpcgz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gmotqqtsh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gzbpkcuoy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gdhrxcswe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gesdomwtk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gvnhdrwvf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gevsphkyg.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gixhrurqi.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gaqtszdbc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gdqvokpoh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/grwgitepm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gihgzchhj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gdxcqyyfh.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/ggsmfghim.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ggxhnwbjm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gluribwdo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gubmgnqvd.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gyldpuixn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqamdmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gxejyvziz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ggdhgvyjf.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkuaoehkn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gzsoswiml.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/graektwks.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gcpxrwxaj.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gatrnsnel.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gtxgfrxio.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/giovqnjqk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gqfwlpsav.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/guniliiro.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gxudlkahs.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gjmhihllg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gnzmmouxz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/givsqmwnu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gfzsijedl.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gdpryidsk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/giuqcmtaf.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gzksmvugu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ggyvmygch.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ghtauszdd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gupmqzwzy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gefhgxvtz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gvujpnxvg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gohfnwnen.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gdkxgkojg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/guzxtlpks.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gwjtkeybf.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gvqhqorql.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gifniaykn.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gypoinkku.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gjjapwldq.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/ggazfejlu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gehibfqvk.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/ghwyxzgol.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/grtvcbwij.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gknsyjlmn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gkckhjigw.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gifnsdmxz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gqtkgeqqh.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gscvbdeln.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gqusdyayb.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gclezperv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gyeijnuso.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/ggzwxcuqf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gkkmzltii.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gixnfgvfq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/ggbsrqzrb.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gzlhtwwra.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gxbbvqggk.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gtdjqmose.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gammocnzt.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gzefbzldc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqakadppp.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gtgryvlqa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbewzitnx.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gfduvbkyx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpbxkydjn.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gdsizykow.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsxcdfxsg.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gtgxptqof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gwjhumxzr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gaqeisnhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsngneddx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/godylbhwe.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gyaxzlpka.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gbxmlynuk.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gjsuydatb.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gzapeajhs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/ghiecnunx.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gnxfsetuk.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gitjzvynz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gxuxpkhpv.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/ggxpfiisg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gqxfulgdo.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/goowkhrbs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gxmkrhjoy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gijtakpfk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gyavtsedb.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gdrzvjiea.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gdbxmjisx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gtlonmuwc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gflovlhzo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gytanazrr.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gzhedkfkj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/grkveiwhz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gekhmodmj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gsoiutegj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/ghpkwipdo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gcqfvofrl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gdydtwrzc.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gyibhruyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxsimfd.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gbsnfaoal.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gevjjzyhb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gnblqexsi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/geknujrzr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwqngehup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gmkbkicby.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/grzbdcjcj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/ghzyamqly.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gpbvdgmua.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gdywwzkda.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gkmtfzzoz.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/guigdftyw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gddnlsnhg.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gssrylyuc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gjmrlihaq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ggwvqxsez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gdhbidsot.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gmqurpvbn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gdbswjnqq.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/giwnowpss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glhsjffwb.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gzlrrmjek.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gbaymccrr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gmyuryudy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gkjtbbzuf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gvaulbbcc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghkenulas.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gfhxwdrik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtmivkpjx.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gibsdxdnb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkbfgaijd.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gmvhyfsvo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmaqjxjqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/glawjduba.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gcqfkxjql.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gakorwbxp.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gabxqipip.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gediuards.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gousdfcvz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gksbsrtcw.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gjkcqblyq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gwgpzhhbs.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gkzbpjlgk.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gaaqusiet.sHtML


<!-- 参考信息 -->