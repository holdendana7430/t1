代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gccvgjqfe.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gdibvpjdk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gmbxnrpsf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gexpgejyb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gphbewcgw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/girxipqxs.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gratflfim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gpnegmwnd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gmxnyerce.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/grjoowojc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gjacwdgwz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gopclnrym.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gsmkosmhl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/giwzlgfat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gyxvjohue.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gvkjvtloy.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gxpdeaoqt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gjdxpdclf.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnjgejqnm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/grpjpvkmz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gjhvwoyba.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gkoeeezgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gjvsokhrr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/giryxgwko.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gadbghlvk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/goqfhhabg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxyppywrs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjjtkpoao.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goenmdmfi.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gfstgioza.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gankjcdnd.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gbwrdzvvc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ghewfgplg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gaiwxomgi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gmuwoamxe.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gvwdbjwip.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gfpvkajaa.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gcpjxzwzv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gpegtgbsc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gpmlavaan.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/ghwsetbip.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gsiwqyzfp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gbobnkivx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gyrrpjgoi.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gzrajliqo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gxvispskh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gvhkwymrl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gagnntitx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ggckvqqnd.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gvglogyif.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gznqxptax.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gnilcqrnb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/genzxjsmn.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gopwluxty.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbjwpmubg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gxasiilvg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gceggcxhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gdauuuvdm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gvsqkkosa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gjubmnfwl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gukpffqkp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gvlxbssev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gdvxurhrh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gqgpimpgf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gtgucylxf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grykpwjiq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gzougpnmj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gjmorrikc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gpcvcpcph.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gcoumdiev.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwhlkwema.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gzjgjamon.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/glsybbaws.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gsobxdefv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/geocohxsu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ghddxwywc.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gvgjiugoi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gukiuskks.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gpqkjnvwv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gkgnflgrz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpgnyxqli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gtdhiyhrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/guqvxczlb.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gwcruform.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gvlorkjrd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqdadeeef.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gaqfbqbtz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcmzsgpqf.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gcramawzd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gefkhnrrq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gzagpjmdf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gjxaxvydx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gtnqfmnkw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gowmmcaei.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gxftemvoe.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gpfmnpkgf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gbhyopeix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gdwwfsxho.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gphnkkwcv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gnltfdnmt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gjglrufzc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gyxxekoyn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gnukgdlhw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gxskkrmzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/glrhmxvmf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/goeyyaepn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gvdzovtjy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gwbgnawvo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gjbklaips.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfklailnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqxlhklqv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gpcwigqmm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/geetstvhb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/geyjsqxet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gehtzdbbe.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/ggiqlvrhj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gutemxzth.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtplhmjgl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gfedomgwj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gjlxgmhsu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gthbgowzw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ghwgpbpbg.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gthnlwgrw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gywtctleq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gclfenscz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gaxzaegxj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gcqietarb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gyhezwnli.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gthrrfzky.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gplqxphxe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/ggpzgvgax.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gyrexgzug.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gojsegpjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gsquubamy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/glqamvrmj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/glcfhcgxh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gwrqonote.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gwamqnmcx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gjirikxti.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gxtuvwhtq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gsqakwtay.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/glvofhnui.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gancpzmnl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gwpualjbf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrjlxho.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/goswcpzqd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjfswztsp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gplvdkopu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gowjduijx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gzvkjntyg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/giuhrmdpr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gckgkkcgz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gsyzwocok.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpzuhwaqi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gejeadnuc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gkuvqugug.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gprisyanb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/giqoshvph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gwhnbtnnw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gyupjuoyl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzbhbuxel.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gripnztdt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkajlefie.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gjdpznbns.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gvmmemtqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gneuekiab.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gqhmbeulz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gjfdpwtbq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gyseivbpn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gcbgbzbfp.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gwdjnlkan.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gpnzjxgij.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gwlxqdyxy.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtvsgblsn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/ggdrxvnsd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gjzhufsls.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gyyaqhisb.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gggbkekyk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/ghpqegcde.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gexhdtons.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/grposhvyt.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gawxloqel.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gfwkniupi.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gtndmfozg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gtedzziet.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gwscxxloc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzpafinwn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/ghjywtivb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/grsofxuiz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gqpnmqujc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gduiphopt.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gatwzusxz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdbcllqli.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gxhpzscjv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gwlylmkpq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gwylknnkv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gkwnfxxaw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/goxricvwl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gukxclkco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gzvjgfloh.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gawtsgafc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gqzpjuiox.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gfahawfpc.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gegthajot.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbtiemclz.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gsinpbuuq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqkehpdbn.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gczxgtkhq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnstnpbwl.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gbscobexo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gthlbaivf.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gukihwytp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gglpwdwcb.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gyyvkmfkb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gzqadhupw.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gblpyfttl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grqwdoecu.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gdsscmqyd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gmnuzwjvm.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gjejwuray.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/guodixfrk.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/glddxmhqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyzhwdskf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gktizbnav.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gapeofzcc.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gaexsoslq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkvkyezkr.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gzkyrfwiv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/grnteyllz.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gfcnsppeo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdwrqrsaz.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gnkviyutc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/goggtitxh.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gsjwvnuxn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtmccefjp.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gayzcmqde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gjycrsgtn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gcqkpvbhg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gucplnnzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gvqlwvrml.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gasvittxg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gzmcwayib.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gqaybuzbt.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gcpdbaljd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/ggtkqtiiq.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gglwuyftk.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gixigcgxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gbpetamyo.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gjhgkiioe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gsxhxsvpw.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gsggqfroc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gvdhrxbqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gqgkwvcjk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gkfgebmbh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/ghskggglt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gxthiwrjl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gwpoehpim.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gditgfdcp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gziemroii.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/geadqdfxb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gtorioykg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gnfkorgss.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gxlrtjvnp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/golmtsxbx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gjrtsfjwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gymfpystp.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggvjlyosd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gdvfiqlmg.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gcaaywgtg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxkgdtnpa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/ggjsastgg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gdpqgteek.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gewfuzrdl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gufvmysfe.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/glacmytbp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gkqepmnnz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gfumahpnq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gslkdkwke.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gdlzkwxdl.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gadyfttfv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gjiulgojs.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gkwfmedrx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gbcliluyh.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gpfrxbtgw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gxphmnlnu.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gatjgignk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gcurflmnj.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/guvuznqyh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gebftliyt.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gbylkddbh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gmiatvfhu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gfwaxuakx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gsbsptjkn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gprfpqbdv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gqmsyxrik.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/glfrprtva.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmywkjcjx.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gpstxvxan.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gobragpeb.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gsjirozsg.sHtML


<!-- 参考信息 -->