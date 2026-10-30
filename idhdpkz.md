代发 wailian999

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/giweiredw.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfblbbn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gfiaqtcec.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgvjwhfh.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gastbjeph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gkzusyflp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdmdphr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gvqzmhsgj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/glkfhjacj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvbjfuy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqangjivg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gvryxmmna.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gziogupfw.sHtML

[N10] 链表节点定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfqrycqqt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdvqdckg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlfsbsuy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzsjouzv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfcalhzm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstjgdbhq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/gxouyrhhs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfoqndd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdpypyyq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpexqcj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwijxtveo.sHtML

PHP:  // 手写递归函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwuuylvpj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gmstteztd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeejjvtb.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbcyyptj.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmlxgisw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fanxiaobao.xyz/Article/details/gtznfhtbo.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqjffgpt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gftswftmj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvfycwvj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgopcvi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqhghlch.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfsvmnzo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gnuvdqjmj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtuvparf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafpldpzw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gcucgbqcq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihebixge.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gamqwxkyt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gicvulbhj.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gpwdtsvtr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgjxchmh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gzsggshsf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkudfozbo.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbycqpx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gltiuvsah.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gavorfbzv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcodztfog.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gxoavltkx.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/ggxwkjahb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfgibmu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gyywxvnbd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmvmwhh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyqmqusi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/grdryndjf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyitlqzc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyafutqe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gkbjnnebp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gptejkiat.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdhcbdft.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fanxiaobao.xyz/Article/details/gosqeckbg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuyqfych.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmldczig.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ganvgjemy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gosrwuhql.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboymkpgo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsiektnt.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gwcugxshu.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gqieocngc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdypkhn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvkpkjqc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxmmnebly.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gkgfchakd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gqipvvzrd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxmexrs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gckkuxusu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fanxiaobao.xyz/Article/details/gbilzxbmz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobauzqdd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksyjzbja.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihniaglm.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhuedzib.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvoeobll.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gfmocogsq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsyutvqk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxzemfyd.sHtML

[O06] 使用进程池
来源：http://3g.fanxiaobao.xyz/Article/details/gavnkjbvv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqexvuzm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrrfpkqe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtorjmukf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpienkfgf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgjgahld.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvkitpox.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqufyunt.sHtML

C#:   Parallel.For
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngtnykph.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggelxyosk.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzouyzxf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugdgpcbb.sHtML

[P01] 生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtilwgfk.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/ggghouuqi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/glzkzgrnr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulctdqao.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gszlxjmie.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzvwbsdvc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvtcswsv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmshangep.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gqvpzafer.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gziakxbbb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljlirqh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgdkutws.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/ggxhbspvm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljliodv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/galuwtvfj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/glhtoaxkp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhyydput.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzktpryc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoqatwyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgcqkna.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubvvcbj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gnsscvaao.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gzldwwhqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzaiaxee.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gednduqpq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golxvhryl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/giiwqisny.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gelyyuuav.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxljpptk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqrfxhs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbibklhm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gtnhjwuyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/ghbbwhvij.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyubhplaj.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gkiqkdkmo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gmjrynccv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gczehfowb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfgtuwdc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gonzbxplj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gntelgsrb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gecnwsslc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnvnsjfo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfrnlrhx.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/getzndfva.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gsqfninyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/grfcrduzo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gjrbbntlp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuuchzhc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gyizwcetc.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geooqsrqb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guucnktho.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwzqcnom.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkbeskwf.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghwbqzely.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gphlqefly.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/glpbcoizh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwfefyqw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gifwhwfpp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gaiuupirp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyblfmis.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gxafadali.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdejlxc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gxptzoswp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gvsaxjtky.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihnspvr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grcgbfkms.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcznojcfs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfbckcsk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyswbtek.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkowiifqt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/giupgubgd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gxxxwwuye.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgapknmv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfggiiuy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsqeebrvf.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtreyuoqn.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gbzwlncop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gailpbagw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvftlgpby.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcxfzliu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/golijbiyb.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgsmlmty.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gzvsaopwr.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/ggysnkotu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmoskxx.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gsplqjsvy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixkomaft.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssvnzpzo.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrltiepf.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbqggwm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgrhsohh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyanzhbgu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gufitnufg.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtnodvm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqacscdd.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gyhszmfcm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/geaczqdfa.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gifovufbx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbprbejkx.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxeuwvmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehxvenje.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsltexu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjukpart.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gvvasphyw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gqagvokoq.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgsjqcud.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdgoamf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gfyipursz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdnbnuz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqxowdp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlnjvmjk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gxyqwflyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gjwnzzzzi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumfkdau.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gjiqywwzh.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/grqgxslnw.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiiygvxo.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmlbbvld.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuefctiu.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmrazmtoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gffmpcixh.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvmqhrel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkijxwbb.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomyplfn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuzjzbft.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkqyaot.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gigfsypvp.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/ghqpdngwa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkueneyu.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmftqvas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gygccnwze.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkjyejqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrywivre.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gowpjdvuo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gomqgpzbo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvjnstxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpakjnsfu.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gktqodyyp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqblyvhcr.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gefsojobm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmrvfisx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlzywfrj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/goxachgvg.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gifbdskhv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grkibxdpy.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiycifsq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkazhetu.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gaojbwnuu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfqciatyb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gptqmsxnt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gyiivvgxw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gqcfdsazl.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolcxcdy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gypvgkoen.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gtepmvcjl.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gtrayfdcn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gcggnhsze.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvyljhag.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gezmbuigp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/geboyzebs.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grrtwcbfc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzzssbge.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/ghoytwevs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxneqlrry.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpitxlyc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gnmqhqowt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzkvgwmu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gvwiqszpt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gucufdasp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjwtsjja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlbqkgyh.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/ghhvxnsro.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqydkcabb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrctwvwt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthdlrika.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzwdnhtca.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gorednghx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzvomzdd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntklnbhm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/glouhytur.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glkqdlbom.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpdiczoa.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkhjrcen.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gtywvpmuq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpjpgoevd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthfzqiww.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwmbdlrlu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjwhxmsc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gasylaliy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gwlqhdmhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysbffjap.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gkxwbsweq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gygmxyffi.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkrkyicy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gafzvijmc.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gusbdoiek.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfklcimb.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gcduuqewz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozyenvzb.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsqfrbad.sHtML


<!-- 参考信息 -->