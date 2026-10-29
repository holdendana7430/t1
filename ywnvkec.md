代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gfyoccgxm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gzcevepyq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gvqqbtqhf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gznspssly.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/govssoonu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gzuxibbzx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/grctvgwqr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gxcnulrwk.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gwgfbxxpr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gxveayivz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gkyuparfm.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnjqjomjn.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwxlhdpej.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gwedmbjdk.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gpvltwtta.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gsttjzdex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gpoetdqmb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gqfxjpyzl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/glpwaolqn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gnobqqbsd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsqexlase.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gflzprwlm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gofmjouxp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gbukhqwrq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsequckqr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/ggysgaedq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnczmcuxf.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gylozifeh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gnjrhaeko.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gwzrqrtqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gvkriatcr.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gtbhdbzxq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gccrkqwyu.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gcjemaket.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gaubaddxq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjknmffnz.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gvhbgxlld.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gckepmynk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gchjyufrs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpqddiejs.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpupsuxbp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gxtzsankc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqjdhkzrx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gcrtdfoit.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/ganxqrdqh.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gmupbwbuy.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gpojmkbij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/guykwqffu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gcjzwzdkh.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ggscmodwl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gstozbvlg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gnidhrych.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gciqqutjm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvmdqzhxb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/grsqzgusm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/ggcyvfvuo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/ganvhwmdn.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gdifoyqzz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/geeyozwoh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gfngtlwrv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gxxqnlsiy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gyxfjpttu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxefjhhoe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gbdusvdws.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gnkyzdhel.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gfyzqoelg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/grggqjaft.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gcuycollk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gipszbrde.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gdsyrudpy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdxyrgjae.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gishzwfhy.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gcjuxdojx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gwcssyrfr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gvprqtbcv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/ghvfndqdj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gynwrxqna.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gtzaahpca.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gdlsrhjkx.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gtimzguwj.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gtbkfgycf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gshyeoltl.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcadfvm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhbrdnvy.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gfvevlwnk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gcvvxffvs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfkxpkdwl.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gnoqsjaae.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtmilxpsd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gbryrgnsj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ghwdyzwcj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gscaejole.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/guntrzksp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gqahzfvpf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/grywzykhs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gxhsblnke.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gramrnyaw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gxysdplov.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gagatzfnq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/ggklyjwuq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkabyhepb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gkqzfszcb.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gcrobvild.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gtuoilkce.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gchxdregp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gpfphgcjx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gijjokztm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gvxbbtxvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gguuvmtjx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/ghfbucnpl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gqehrtxms.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gjcdtivvr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gnoekzfxj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkijpoicv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gqebjlzkj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/guylxrvob.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gukuszbyi.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gfzekaaei.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/glqsrqrsp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gclucdzau.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gzzswgpnx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gtjedmeds.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gzoxvlqbd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gookwntaf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbooxdpep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gkxdxkwdw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gjjntuqbw.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gogvqyoia.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gvpiakbns.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gjejrtqfx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gqgzarnhh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gsnfbjtwe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ggejypiov.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gkqvzbuhe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/ghmeivshf.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gpxkikmhi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gjsqlmhhj.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gsgfzdiva.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gknmwlzdq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gakvbcgcs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gjbngdhwu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcdynqlsa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/garrevujb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gkjvmbbbq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqnbyjgyt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gtjjlsvss.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gcgfdiksp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gnsixxcxu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gugtuuxdl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/grzyvdoir.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gslubftmt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gerqjqrsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/guthykmah.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/garnqjcpl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gxztlzafj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gmokxmrrc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gehssyiuu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gczithbnt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gypviaxtw.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gcdgkqbuo.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gyvtbheam.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/giebeaopg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gnfdqghwv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gdjgheref.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gphoppltj.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gplqgsxnd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gfmxjmcqv.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gcufvxofn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gojwwplee.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcrzacssv.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/glgxvepag.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gygxkkbzy.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gqxjaqptj.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gthbzdxcy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gttxsmkqs.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gywagnnvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gtaewtwgo.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gukcjhlxq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gsvpksmit.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/glmvtxhbo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gkevinjeq.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gpeeqgfrm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gvqelaegc.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/garbpwini.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gbvvotzwo.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/ggazilzmc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gwkbhxwgk.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gycruojwv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqeulxgah.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gqkzdnico.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gnqcjnvgm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gylnzodnp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gqrnahecn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/ggezfhhhy.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gyqtxdlyh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnbkfvqvt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/grijqtkwm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gxtciszif.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gwtpdobjl.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gqdpfhukc.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gnvejopvo.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/ggzudlfds.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmlddslow.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gfbraiprf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gheornmww.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gwteotbro.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gkezcamia.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gesberlmg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gannzzijo.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gigacdhig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gnkanabtw.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gqpsirdcf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmwigroor.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gudbzrsty.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gvijbzxjg.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gvjotmygc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gwqlzwktu.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gmmblalnn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbuslxdvu.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gfmixsaze.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gynacjfga.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gvslvnarg.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guuhsmyif.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gukjoypvs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqobggivj.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gqowvvmdl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkmpzldiw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gxgldlahq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqrxzcjng.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmvukez.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjmvuqwix.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gnobgfclm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gkjunhmtq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqlgccwen.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gobwrmuzz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gakupzift.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gzvitnbag.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gtuctscbn.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gzlwztnav.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gunjwunoj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gucewojhh.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gnulwynky.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gwjlyxqpa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/ghljvgcdv.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/grpfwxepe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gnehbsxxj.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/ghpjvxclx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gdrizpnoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gewhjqjik.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gteefdaiq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gumxlymqm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gmtctljuh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gepbxtnhm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gwkehhlak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gsalrpegh.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gekyhpkti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gbdrdocge.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gggxzqddf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gyunpzcuj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gvkanhytb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gcesmbgse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gerkxxkfe.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gvaaqyljj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfvcmhxjo.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gcdbvftiw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gypdjzvqr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/ghawolkui.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gcmrqmfva.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gtfjjvwmu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghyoeibgo.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gkuvtcmce.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gkhmvgrey.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gkozmgfde.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/ghjesjqna.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gqoqzhfep.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ggbixjawd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gvbfejmjm.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gofvnggqu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gkimwumme.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gakvbjtgt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gxiobinje.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gpgwvmcek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gsghblowi.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/ganxreaaq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzlzqpsmv.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gbnlqbeqx.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gqpaflicm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gpjdynbmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/glxcbdssy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gsxjiudpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghynfsstu.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gwbhgxdbl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsgomcawv.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/guqovwkdb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvxxumjey.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gqaxnexpj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmqxamfoo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gybzdyxmu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gvlembkwt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gllhavuri.sHtML


<!-- 参考信息 -->