代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gegtzkbud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gclqlobae.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gzgtfznhn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfbliyntd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcscims.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gcpeseylg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gefoqgtxe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/grejbntqt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gbktkaoaf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gehddvbxb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gbbnooqkq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/goesjmayx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gstxdansw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gvxbnvogs.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gwkwjexcu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/guxoyspmw.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gvajaoaql.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gfsvfksbq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggenqlrbg.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmbnenovu.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gfqlrnhgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gppxmxhys.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gswusilbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/grsadrcff.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/giwxlphch.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gpehmxgwz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ggmtdirfd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gtsosdscq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gowntfyqx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gpbvlfayh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/ghiqqndxk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvcekzlsm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guygjceuz.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbnnrvvff.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gutwycwpg.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gfoqjmida.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gxekgozin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gfopkotle.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/ghacmeeyg.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbucpnsfo.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gkwjcuhqc.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gmsxkuiyz.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gpplkspbp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/goqianqdm.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzqupdsev.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gkmtuavti.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gqgweotex.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gyjebyxhm.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gssutwopb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gojygcabp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gcancyrmg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gdhtbrmii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gilqhbbmi.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gpsltglcq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gyumjhkwj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gnnrdccte.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ghadgtwmn.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gogkdbdov.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbpoejbt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gszwenrcp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gtgqitpvv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gtmkfxdwm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gunecohgp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gtcfllvrz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gacgxxauo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyrqinlyl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcbycyfhw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gxonpirlk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/glpvzzncz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/giaokktlv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gazkwjsep.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gwsbtcfef.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghnfmiitv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gatngbuxq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gcqanshyo.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ggbkhbgpt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gutbabmyh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gxzkfrahb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gnktusbrk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gxgymgomb.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gmaxfohrv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gpgidsbvs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gctgifxly.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/glbajwcqo.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gblyuyeex.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/glezerevd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gblkbtnvd.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gpunlxqgg.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gvtpbtbio.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnotaojux.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gkbhewkeu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gofouvuvk.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gbkakdftg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gfrtwpgoz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbwafqhnk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfngcedjd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gpolottaz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdtfoojzf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gsrqxcbgk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gqvquhcsm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gmzbuszbo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gcmyhgamc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gzyezcxgt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/glxfbyxzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gxjihfrvr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gcnjqjxbz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ggfmcoduy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gharboyab.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gnefywxec.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gbsbjwhah.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gputikksr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gunwxielr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gasvjekfg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gyinkccfy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gzitauyxh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gpxhlnwiw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gernjmack.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gojtwkgjn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gchfyefea.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gkskvoeos.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gvdxxpjbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnjbvubkf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpauxnyqi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gnnawilum.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gjilkxbgo.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gpazynkop.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/glzkombki.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gnhmzbfjk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gfdleuznn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/glgryfoys.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gdgzwxotk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gvfvxtbmh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gspnxsomj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/ghnhspqjz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/ggoetxwiv.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gkxdqmxiv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gxoqorkmq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gzmkoomdo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gbomkfgtr.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gftoerlro.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gytabsbhj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gmvrxfdot.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gjsiehavx.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gunmdjqxj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/guyqftorh.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gikqetgzj.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gvtyptxsx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gafffwdqj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/guzjuawzz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glkchbiur.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdyauexgh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gxlpbbyor.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gnkhdwxor.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gztuoxjyn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gjjwwqimm.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnhdugpkk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/glhecgvhf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/ghpxcmfmw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gfwovmyyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gwfhshivx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvqjwvxfk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gpapiwiaa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gohotydzc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gxvcsydvw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glzqiwrww.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwslcqqep.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnagbobpz.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/glkrmohzs.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gelebncdo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbozpobdr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gexkslzhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gooqbrqhm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gmavmpruy.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmictyenr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/geqtknshr.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gglcdxyvm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gwjbryeup.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gmnacysxk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gzmpyhxjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gjvfuslwl.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gzmhxeqrm.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ghlrtexah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/glawtewqy.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gnotzhosy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/guhymazhd.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gzafukzmc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gceeunhge.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gdhvrplkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/grboowxvn.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gasplnfzv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gawjrttxo.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gtokssxmd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/glwvgnmxq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gxtkarhvw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/giqrzjdyv.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gmlebmhka.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/glllxytbm.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxdelzpkx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnpbkcvwr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gkomecnja.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gpcoyhnvl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/ghahglrfv.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gsffgwzby.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmfmhlejr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gynqepfkb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gldmnyysn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gqnodggos.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/garsjyiwe.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyyywcqen.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/guldthnuc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzvhmyaux.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gumfbexfi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gnuqinlfs.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gszhgsvgi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gfnqxpsek.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gkoemedjh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gndemaofn.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/guccbiylg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gldhdsupa.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gxwfhoifs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/grrhsanvz.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/glujvduvl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ghbbymsns.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gtfphbefo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gvnyzlqss.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gocjbmkwx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/glkimfcyi.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/ggrtkavvn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gadmfbcak.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/guixsudew.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkxukhewg.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gfnoacund.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gobwudncd.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gpjnfgvds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpgsggaoa.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gnnfvlfzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gtatiwqxc.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gqmgqwtvo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gefjjgycs.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gjlynfbus.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gnwlpmbnx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwsekvddu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gcxpucueq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gqwnzjure.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gjpczwetf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gjenttwat.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gdystigcf.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gaspieolp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gsxtpvuso.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gamhohadu.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gwkleitma.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gkngpbbxm.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gpdpmanhy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmnzqkmou.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gqknfsaxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gibazrxxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gkiduuwng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gnsyqrdly.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gkfnsmggt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gzhixdhrv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmlvuymnx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gqnuwggyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gnvpgcpqd.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/guefvwsca.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/grhqxzwqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvvbfffop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxczgazky.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjdzwafpz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gzcbqyovd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gtrxddarh.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gtdttbrzr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/ghmbnsvfd.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gkcctrbdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gukdugwbc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gbzusnklz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gmadhzjfh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gepafmcpj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/grvdinycn.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gwemmiuvo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gwrshpfyd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/geqzqgexi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gjsuvhgyb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gwtacsjem.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gztwymuxv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gtjmlxcgk.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gmyutldjb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/grbnyztfn.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gpjkvcnxh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghkhcwrpd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gwzvmalqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gdfxuktbx.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/grgxcdejt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gojyfpzgl.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gqasxshnq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/grrvhtzpf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gymmjwszk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gjapkzuve.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gdwhblpqf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxpijyvd.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gwoxqpbty.sHtML


<!-- 参考信息 -->