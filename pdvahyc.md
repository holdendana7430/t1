代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gqkvvtfvq.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gvdbzndmd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gbqmojwrx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gafazhgmf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghdcrwqpo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gtcgufchn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gnlizyrfm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gziyawsuw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gymcuwajs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gaearmvdl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gssccevjb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gyxaypgwk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gurboukuu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gorlzsbeg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gnbknrymi.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/giwmmbvgn.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggwgckfxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gdfreqsbj.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gygpghyym.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gyfqcoeqw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gjlwmtjsq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gqoiiwalk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gsrmatqpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gqxwwfsuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ghcoypebp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gkxqmxfnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gizfiifpb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/guzmmkehp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyuyxxzal.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gbcaxsuaz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghqgifybs.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gahjnnwsk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gebhwfatm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdoqedljd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gbuzphgws.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpazdplqg.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gyegpwgde.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gyjcqnurb.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gccckvxhu.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gigzwukmc.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/godhbiljl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gpxwdartd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gbnyhxlsq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/grbipzpri.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gascpmtto.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqjxwfry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gkylndllk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gtqimusmw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gemffntoj.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/glffbdmws.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gnggjyllt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gsxkjvawy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gxirkkvbg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ggeobtyad.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gfoybojma.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gsuedcqfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdphkvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gotnyjukv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/grvuqilmy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gpqzoaguo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gzwiiyzuu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gdggxnmqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gsaohkolo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghklhpgan.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gbkdbvfvb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gydkbenzb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gkfxdosxp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gbfbkjzkq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gbccwxjav.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gbqamyfno.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gliccvewc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gfvboigiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/grdcspbzp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gmtxnylfj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gkjvcqvhd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/geibrawov.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gqxoutwvm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtnitwhmb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gapdzdqhd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gbtiivrls.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdeatujje.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gslhbgxvh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gncidvnql.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gucaovmtg.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gbgmblwij.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grijrzswa.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gxwnbksua.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkxkgutxi.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gdljzfjjc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ganuibhyr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gtqmznefg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkbunwqyq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggaxtnqkh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gywcnqzkt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/glshxcfil.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gfodsuaqd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gswavgosc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/givcbygky.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/ggkxvrfwz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyodwhcg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gwluwpkax.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gkybawwsq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjmkbqyzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/giymgvprn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/glvonnvqj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/ghgvocgya.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gvfqzfmhg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gxfbqixvu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzjozroni.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ggsowwnbx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gqpgklbyj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gzckrnxub.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gqnjkjstj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gzxswjcew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/grawqdznu.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/ggnpzlzpn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gnnwrekgn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gblogqbex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gafxzasob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gmriukfcb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gooobdalc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gdndfkxzj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gzffocogh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gascsqnss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gwyydmyxq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gdjvcrqwq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/giqoltolw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gkwdkxbof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvsjoaeug.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gsplwhsut.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdbwbsyqh.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gvgzwbrsq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gzjoqxgjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gejkgwmjf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gwukuqlkm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/glttqbhbf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gnhnnsntv.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gaqzmdayz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwxmogdyr.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gedmqtude.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/ggrijfobr.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxltcjzpi.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/guekvxunf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gwijabfrw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gvrclhjtu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gmqdgkefj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghuhxaber.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnvgcrgpw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gjvnuteck.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gfzqldkpi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/grgskyjje.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gvxtaxahl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gqtcutynq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gubxqlxsk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhbnqdx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gyoskdfqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/glkjjtzxi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gikzikynk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gwzcdbjlp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/guqhwnjww.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggdvojmkg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/grvsgblvc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcldhyejn.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gtvrwtsfc.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gycfffavr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/govkupjjx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gbbqmnhje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gregwnreb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/glteajtgf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gultuvsnx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gypbtbimg.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gciqcsnvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gyhucudpo.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gbwylljha.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gamvsgezf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gycgdzydm.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gtyqxfdih.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gwepleyhh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/geqftushm.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gojkwjnnf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gvvazdomy.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/goknnejcl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gxcwdvyyk.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/guennkhea.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gtziodkwn.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gcdiccugt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gqfbnykyj.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gosxhbfic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/glpclatvg.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ghnupwqxw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gwlzhkmvh.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/ggvxsbucg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdoskvhpo.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gnswcwkhg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gzzfbzpql.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gkdssemzx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gpkakybxy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/ggxkqowbg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gwaqccoxd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gusfhzidy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gpibyvuhb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gipkptaid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gtzowscsk.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gwhxwmjbs.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/goxgfglit.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gslkedjmf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqoujkqcn.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gjxbquzhx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gnlxsfbdx.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gjehuvjlh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gdjpbuhdm.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gncvphopx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gapknznuk.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gnzcxknek.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxcsfebkv.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gyrsuaqjg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gnvtuocdx.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gkzdbzdfg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gdvzjktgs.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gjetbrotl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gugabehhi.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gvzraejvm.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzwqivcqj.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/grmuaxlxq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gppxuklup.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gzaescmiy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtwlfrtxy.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gizsmdtzt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzpsacazp.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/giyokzkpc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gondsfooz.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gtcxatkpx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggwonkgta.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gzehpresa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzkljsgqc.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gxxeoppow.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/grsfqkxsh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfhcllepe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gssfmyfkn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnkwgvu.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gwwniaauu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gowrmlvar.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gjetzsydi.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gcdnzwdbf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/goxweyrdx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnssnhezi.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/guopcbhjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/ghyijadgy.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gpxwmoilf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gjhapdzpn.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gurjqyggn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/giawoegwg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gchaickkw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/glfjrjzds.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gbwveoljy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gdsnefqzp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gudclafvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gcmzfaira.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gvlwqnxrp.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gbxdcuqqk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/grqjjdqnr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gejgmojix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gezbbkvee.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gfpqgyzis.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gbqiwrffs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gglukcctt.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/giwhlgfbl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/ghuqclzxv.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gidmlfqxf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gwqpsnuyn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gpanwbgjb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gsvisztso.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gsdjzjhps.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjvkvktnf.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/giflzolxc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gpkwtajky.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gzwjkqcnq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gflaqekbd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gwclctptk.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gljnbeuhj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/glvplfhys.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gmakvrofr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gvbsvhsbm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gmzdxkubz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpkqczsgp.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gufpgxxzz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdjshdbkh.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/grjapppzt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvccnvniz.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gkmdnqsjt.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/ggryxpikp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gygwjssmn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gomzgptsv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/givmmqift.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gknmrbhuq.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gldkzazkk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gemjmvotm.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gftyizhtp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkjcvvtci.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gdglkltth.sHtML


<!-- 参考信息 -->