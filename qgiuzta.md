代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gjhannimw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gzwiwpvql.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gsacvtreb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gafowcmvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gtkkloswp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gwokiayef.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gnbffivhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gpxmexily.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gquotnmwk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gwtlagmyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gieejemph.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcarwatnk.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggdhsjyld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gileezayt.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpdqtghpv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gabtxvjqe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gszhttvmm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gifyntrmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gnfeblcap.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ggawwquyw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcmazkdop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqmnxqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gudtteikl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gdnqhrjcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjvkfsbwc.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gjjcssppr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbrxyjiea.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gcvgkwoud.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gwrdgntzu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/guwwfbgpv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjlzsciuq.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gwkpoixwb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtevludsg.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gtvhkocph.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gohouxdwy.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gtztxzxft.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gcdmvhoqk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gnutftaid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gaktzzinr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjduyxioq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gleakjudb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gnngzilbu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gqvbosgdp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gzywuqqsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/geofapjxe.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gtapnxwqw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gvvpbpxrz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gkyvpthle.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gxdogwkkf.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpgspgfsy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gibmihmtd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gozsikyik.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gdezsxocf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ggwbugyvy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gvhzyvqph.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gqxkvnqdg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gurxsryzt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gslrddxor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqcrpxhda.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/guqgslqix.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gkvwwqcjy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gcrzmqcxx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/ggbpxdjtb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/grjnzubii.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gfckivslc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/glwjvlivq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gevifxtvx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gxfwjqgxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtemhmvdi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gogpauhoe.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gafqckmer.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gpexnycmi.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gedseyhtd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gzrveqpkt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gomzsimes.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gnxeenrcd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gaefpwdsr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/ggfhhirkn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gefbwesna.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gjkdtasya.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gewjrwaay.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsbfueazw.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gviezygic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gubmsbczu.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gsovlyypc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gkkgmgllb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gaqpfjpey.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghzfckevy.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvgtjcjhd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvozjtq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/glxwvbooj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gryxnshyp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gwzmqnqgz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gfswrjetz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gbhghdttc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpgdoxgdp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/ghxdufqwq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gkfsgnuic.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gufhzhlez.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gtboolbfq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gpwigxjcw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/grultttub.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/guvtjjwdy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gxkztgsdt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gypjzgzau.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvtqximzz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ggwpompqr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gnufpfdbs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gjgefirnw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gruvxdvmv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/grzjgnwyc.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/goxiopdyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/guggacnci.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gcmgbqryt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gspuehdxe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gybvbcxff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ghzgftneb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/geurjyluc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gvybzumuf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gmlcjxrun.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gozlcsuqa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gfkkcavum.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gxpobpnvh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gdgzdevkc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gzfkqsjwf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/glmqrihcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gcnevmmmh.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gmpxllqzh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gyifzehet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/ghfkwlkmz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gfavhqfso.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gttkrhxpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/ghpdqvrqj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gxwpmaadk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ggsyrxihd.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/grxedbxif.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/ggfrcnizg.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gquwsnfco.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gvdqadgzc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gzpwpvalo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gwxftuzht.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzcjtrvbd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbbxgsmzu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gntstjdbf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gvyaywvar.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/ggyhulfur.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/geabfqdgv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gmboxjpie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ggjpmalcx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gnmsjmoiw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gqbxpmysn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gqbfwxvzd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxctkfz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gmvftizwp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gexlndmqs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gyhmffqzv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqtzroxvl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gekpsxowc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggcktdmod.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/giwlmwzze.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gyncszffj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gjyfibiwt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gajlhexwg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/grubssbug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gkawmqyik.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gabcyxcyq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gkxaosgws.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gzxilljzz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gphnjvals.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/ghoojqray.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzovmme.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gutcfkywv.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gyrtmocut.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gofimrpaz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkbbakbth.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gsiqxsisl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gjsawycam.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/glcljxzlq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/guqiqzjpv.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gxgbuzopx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/guwzzzjcd.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gajufkolx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/giordbnzk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gnfdujplq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbpdxgham.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gfyfrkinf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gykrcgoqt.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/ggunagjmh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/grvvhtbew.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gcqrpvzlv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gphatmyeo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gooosqjta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gsnvqaqwx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ghsljaenz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gunpvtlsu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/guvqpjabu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gxpyoqlnb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/ggaudtgvc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/giapabzsc.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gdyykiedu.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gltqlowyw.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gsnpdctqc.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gplpakpys.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gdnpyszqd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gceyiouhm.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gzqqjsekw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gmjqgojpl.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gepjozjyl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gczkyatne.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/ghlkueldi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjklulewv.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/geksshaxx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gkdjqhsan.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gmnjaxlet.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/ghmeiukkf.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gozjurcnn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gukmyqawc.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gazomnzlw.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyztvdmok.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gbtoiljfg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gsncifuoo.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gqgounluy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjgvghlvf.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gqrkcqmpv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gndmcptwp.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gperrbdwh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxvbpnzhp.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gmuoxdeco.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glrayacvj.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gunmmcmjn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gplbwhpxy.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gpridytlr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gcspdofiw.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnovlwain.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gaxbcfpzn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gqfxnlccv.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gybfgwwhi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfynsziff.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/ggifkiyrh.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gtcmfcfpf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gmlwitkqa.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gsiarsmgr.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gorpeonyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gqrkngvoe.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/grvwerqoz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gulemdfxi.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/giwctkssi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gasbvzirb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/ggcercrfq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/ghpitdavv.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gwgbjvxer.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gffzgpenp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gqktnhzpl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gcmpanpjy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gfetaeryw.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gpgukfhoz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gqisnwajj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/ghgcijkda.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gbxfqzqeo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/geeznccui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwcbcnjan.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/guqspiwwz.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gkikdfwrx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/ggaabjnbh.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gnpkfhokj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gtbypybed.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gsqkukvxv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gutqphhdt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gxwhmzlsh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzfqjokca.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gqqjzyenn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gdxdmtvyz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gmoqzsmsu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gxogymqkk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gvvvvbuar.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gclcfjmdq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gqzdzercc.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gvkqmaqgw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gbgdxtjuf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/guchcbmbd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/ggonnktwi.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/ggqxyhsyk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/goikdbxxf.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gqaeybfft.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gkkpepqwc.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbwmnyrlz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gvsmeyuqv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gaemfsvxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gglkyizee.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gsvzduifw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gqmymaxla.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gokervogf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gamnzpsxf.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gpzreqyfk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggimmckki.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/grytgahbb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghhtfuefe.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gvtjarehi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/garvszqrl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjdmjfdmc.sHtML


<!-- 参考信息 -->