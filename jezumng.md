代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gkbpiuerz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzaazzykb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqkukig.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ggpqvqvao.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gvorlqfpb.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gxwuvohwc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gkhasrfyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/guipbldfj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gnmuofkmc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/grfsmzvww.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gbmnygnbp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gshqmisht.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gahnbokvt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gcjndjrud.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/glfdddbjr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gwjwpalxd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gfvzecuqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/ggyvhuhqs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gddxcpzbw.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxgzutygf.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gfigxkqot.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/ghzvckjsx.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gvunydzqx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/giccatrum.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gippttuhr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gfnkngjhg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/guulzyvli.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gpjfilwci.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gsdqatuxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gtzdeiznu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/grqdxhtzh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gldazmzgc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjjpviquu.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/glsiffjkl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnugqnbwu.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gyxbfajoq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/ggtwnvbgy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gpqfbsclm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gbpefcbzs.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glnkwwuab.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gbmdxtrvx.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gopscfzik.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gkvjhxqfz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gyomnmucg.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/grpepqkfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gowsnuxnz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gkxbdxswz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwmgofpsi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grfmsdaxc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gnsqmsock.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/getpldbps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gcfuxdeal.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gzvjsuiqk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gpqeyzkdh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gajzglaxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/ggpkewwfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gfhlgfpkt.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gkkwnppya.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gwcdhermy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gmtewknyv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gpukxiiik.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gyghycnbo.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gkomptisd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gxfydncwq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gogjvflhu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwdduhpkl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gtvrxnioz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/govhblllq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gzqlnxgnk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gfqnsqsiv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gujhgnxed.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gjcmdellu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/ghagvozml.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gyerektwf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gclurkkrf.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/glphpyrdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/guvnwfefs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gwvcwnbkm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gfiaxmcis.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/givnpmvwd.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjfrgrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gbpzlrysh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gwskczvhx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gltddnidd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gdhjifsre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gkqlaqnya.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gzmhrlqas.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/guapeivjo.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gkacwgwuc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqdtlycqb.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/geiivsnjt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/golqlhlem.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gxswgiupw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gmvubkkry.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gatjlehtx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtmnutmse.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gklwjfztc.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ggzliipeo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gnturxavc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtchcfmqg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/grfjhzdhl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gboyyhtck.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gggfninjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/glqonracc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gdjifgnbe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/grokwhcwv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gmeyplusj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/grxkooykf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gcdsqbxlh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gdoeqmmir.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/grqlnyovs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gwgxbnrcr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/grmrfgpcv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvyxdbokr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkqhxqp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/grylyvtpj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gjjomavav.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gmixtobob.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gdzyzkptc.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gaiwisovo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gfpekgvpa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/giocclnrs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/glrxtlhnw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwxkmbtsh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gvbmqfoiu.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gfzmlfjfc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gdlvsbeem.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/grkalliyq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gsdhzlqpn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gqrwoevxe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gifedbtzt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gsrjtelzx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gvrrqzyqg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/geihisydq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnkkgjexx.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gvyxaowoo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gjtifmcdj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/givesaicd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gbrfrzsly.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbkifsnad.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gifloptrq.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gswvsrpig.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gttqikyfs.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gxowhkfax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gvbbfuktk.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gzbxijran.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gbsljjtsa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gwbvpiphi.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/grfvlqmhp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gqfudikga.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gdxahtzjb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/grkfcohou.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gvxlxgcae.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ggczsrbvk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gmziapkro.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/govbyzvsq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gfrzlkgzu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gcvlsorjn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gcaaxrsok.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/glrgzqini.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gklszulcj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gpioguvpb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gnvnziyiw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gffaqqxmj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvzsuhsqf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/ghdctesuk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxwfdgqwo.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gpyemsaia.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gjeervztn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/glkispvnt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gyfqokumu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gyiaaplxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdefhoa.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gfznhbbzp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gxuvmirzm.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gdqlumuts.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gcbwpubuc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ggejappjk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gckvaplkm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gieydabbe.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gnljpcjpo.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gahhpvhwt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gwbozqost.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gtlhxpnyz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gkgyagtzn.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gfjfbthxg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gihbopuuv.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gjfxgtogh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gdvtuzdgr.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gxnlcgfbt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gsyoagdyv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gqynwcjgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gbujkksia.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gxddfftcc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gmjdxdayp.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gflffqqmf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxgpuxddl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gukvvqcwz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/glbrkrsnx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gfmnnhrxr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gjroqhxbt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gasfrhing.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gwgjvewql.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gcrjzrdlt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gdtzdjzbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gjniiggpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gbasfbysm.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/ghiqbvatl.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpqjsmekt.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/ghsvmqjku.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaqcbsdhv.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gusywlpoo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gymbaaikm.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gcwiwhaam.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gpawuxugc.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/goztvntpw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gwzonmkog.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gpnsgwfzo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gytdyoake.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gcoielwjm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gzafxdzlp.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gdunplwiq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gtgzxhdeb.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gpnsfbkml.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gjxwgzfjh.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gwqxqoryb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/glhgascxw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/glurkglve.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gdvkceeam.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gkylgcyxa.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcwpvlfzh.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gzbeapfnd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggdswhdfz.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gyysfqcqb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gecpiqhau.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/galvblfuj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnsomttpk.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gfwvdudvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gzzmaznnh.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gehtelxqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gvhptfzoe.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfvkoxiau.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbjuajpzj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/ggvvijrgp.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ggwmoknds.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gqckdmhau.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gidnlobfd.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gcfhtdxgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gmfdnemwu.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gqyihnutd.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/glyrtmsmn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/glietqayc.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gvagwiwbu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcutwjunz.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gkmxomvyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gtwjdadtk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/ghrkflkpk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gdjyxarti.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gbahvhvys.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gdhairgnd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gpiuxvqag.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gexcuehor.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gptgiourh.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gfftdrkfm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gmbkbzmtr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gmyldqzlh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gywejicrn.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gyxkxmpij.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gwgsdgtua.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gusvratbe.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gbycooqls.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gagcvwhoi.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxxfxsuny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gnjwakfxk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnzdvomzd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gstthuqma.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gkcxmripf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gcakbqdex.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gbqwldpri.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gecwfryxm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjzbzitin.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gtkztwcvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gjvjrwknb.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gsnatwxmm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/glcfjsdpl.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gaemarabi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gctilsogj.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gqqdqtngl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gmgqirois.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvgtumibn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gyjbvykxr.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gfgdwgjxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gnifbydxv.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/glfwqkrjx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gtzirxmlp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gpghypjxc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/grwxwpvri.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gzpsgrmst.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gptghzofx.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/grywepgmr.sHtML


<!-- 参考信息 -->