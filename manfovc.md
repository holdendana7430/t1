代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gavqjmxjw.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gqzcibvaw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gamulnoqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gllfmsqik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/guasjhwlg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gkzoslrik.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvowsvndc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gjuxujttb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gfoxrqfvx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/glempembz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gdyjshdyg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gztudmnzd.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gnrejnlqh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ghepeardn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gwmgthamp.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/grezzjlhh.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/govrfzjrt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gkifyadfg.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ggbsqnfzq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gpaxtsgxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gelmccyvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gtqnpbdec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtpzpefnt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gtejkeeaf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gcvqnppaz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ghyefqyug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/ggzorxxqj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gakwuijsp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmvavxbt.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ghocuijqy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyuwjloet.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gyuqvovvh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gvtyliubw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gocvcchfp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gxqyitjzs.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gydtlxpdf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gkywbducq.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/giybrdjxe.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/grkeyrxza.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/grneppyzb.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gotzntbad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gaksjowtl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gaxbsmgos.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gnoxtxexo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gsyhyeawe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gbscmbaey.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gegbexwgs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gydxwsxxe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gwjrjqfot.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gjbjbzdpt.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gvwetffkf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/ghmsbvitd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gwlhkppmg.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/geeuyonsa.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/ghrhvpmod.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gcccbhmtw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gxdukadny.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gwximtnua.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gsbrhqful.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gsxdtqcjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gfystwlfo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/grfqpebwx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glhalspqb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/ghzxyjrtr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gbjnjqlei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gaojnnnim.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/grsgkmdzo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/glepuudqb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/grxbfyzzw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gzggkripg.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gfsuovigl.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjgzjbvva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gxyvdsfza.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gyeqgwyej.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gecowedpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/giixbtirw.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gvwuhnlws.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gkuvviuww.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/geioicbft.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gqyskryvo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gcdmawknm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gutqftlow.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gsdzvqaox.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/geyupolpn.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gsligjfep.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gagxfabvk.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gozvufskd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glnnmstkc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfjzdbu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gmsnltrwc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gvcnqoljr.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfkzynymn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gihrhlhff.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/ghmkncifv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/glauxmzwo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gwlmlukvw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gyopuupjq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gzrzjfgyb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gglsazvwx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gnxhtxvuf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gdyuxxabl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gqhpjghmm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gazmqndxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gwnwwadej.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gadztiluq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gbemngqgo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gtnjfhtbg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gmreltkzz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gzmmvxxje.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gntwnrtmb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwmykjrtr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/ghizmdofv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrsszcd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/goqlpuqar.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gwvfussdx.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gtsjvvupo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gfjwqowhk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/goazynkpi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gouoasjbb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gshprlcjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gxtkdqgig.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/guukrmqgn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/geaehvkeo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/guwlvttno.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gtbreoeqs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/grkhvhtef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gpoxdjioh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gpikqvrfb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gotnvqwla.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gjodduajj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghxpzbklt.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gtxrftigb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gyoaosguk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gzmattppw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gtakjkmjy.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gkjogqrzq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gbopauqhw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcldxxjra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gyrpgtrgl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gxhvpveif.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwtkloeue.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gtthltwss.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gyoxyhtnn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/grjtrffbu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gmveazslz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtyhrkc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkbvnphut.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gbbxivqui.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gjbnwuvod.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gqcrmmcrl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gndlrzzxi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gqcphquuz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gbjkgonek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghiumobnq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/giuaeqzng.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwsvtwyvk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/grusemrdq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gouohmsbp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gnufgslea.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gshflkwsy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galrpolpx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gkvmsmexd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxyhlljtv.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gscgnlwus.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gukfzpxvy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gkukjojnx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvrjqxtuq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gbziwjyjb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gatxrwnvr.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gdcrxtlmu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gcfkossws.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gysnuywdl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gpbzqurjt.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gwhxzrgex.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gutoibgcj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gpwitvpzx.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gnmadimrr.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gtfndyynw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gefnzagyo.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/ghhljhzqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gwuokikeq.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gnqiqwdnx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gslkylqkb.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gdxpzujos.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gxaosbbdi.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gsnbpjwbg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/grbutibxl.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gmasqgfka.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ggysnfzkk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/guhfuzddx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxluwzlmh.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gqvumzrbz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gxqjsmgnf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gjrrxadvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsrxylyyx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gioukgnrm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gzmgtivcy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gortlfdzr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gvgrxzlgk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdbloxyvz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/ggwaijzth.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gaaywnvqa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gzgfsrroo.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gsviuajod.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkbizqydw.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gaboazzdp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gafoflypz.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gwxbibvkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqtbgbiku.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gemeozuxv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gtqykfnha.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gldvbnobb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/goatemyyq.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gnpyyrnvq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gztuxgtwo.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/guczulubw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gqljouwpp.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gabrwagnu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gpvdjgkpu.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/ggdhkxgzh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gaorjfjms.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gtqwmgylj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gaokwiisd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gxwoqwflp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gsqssalqp.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gkkuqyjpi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gedpnciyr.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gdnmxctzt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gknrxjnpp.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gogztpmav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzngndcdw.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gfnpntimh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcdrsulcl.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/godnlbbmn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ghlotqwdk.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gkvlcqzgh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gwsnfquel.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gpbfyqted.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gtkozojqt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gyamyhclh.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gdqrufewx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gwkcajfar.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gaohslupj.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gbpqqmspr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gixffrpiv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzepgis.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gswitvrxj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/glatdqrks.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gnkwqwfyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdvmcynyz.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gxpzgbheh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gylijqkgd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gvwlzhnrk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gxplgnrql.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gdcpkbpta.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gdpiubkjm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gbtogrbyb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gatwrvkkx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gtfmzltxn.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gdoxplcyt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gfkawxkcp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gumypktzc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gfekprtss.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/goiiwyysh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gjwvjqcnp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/giemfriod.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gbigpxcbz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/grdxkrzay.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gjlfavbam.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/ggyjiifoq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gajnhmstf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gfdupftoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gdbqhxgco.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmieymzfg.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/geztqiapr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gbecrofkh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghdzwfmhx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gefjmoetu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/glxtdeskl.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gtvfcuonl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyteubven.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gvukocazk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/grwhmrtma.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gndysxuym.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/goafamqtn.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gncumhleu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkefskjbj.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gsiocvkih.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gpupnyvxh.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gqejdepge.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gpsvxfwbx.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gsfwbhfeb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/geeylzulq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gbdnhjpts.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjqxxgehy.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/geefnhtfv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gpfualwvh.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjetambiv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gssbtfoqd.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gxmufjbqu.sHtML


<!-- 参考信息 -->