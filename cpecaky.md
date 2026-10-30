代发 wailian999

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gebgbayed.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqlnjegjk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gwybnvibe.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqdviisix.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/grdwbsahi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzekoqhxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gdjuuhauj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvbirfkqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gsfvctxgo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzzqjgmcv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gowfdvnai.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsmvobayr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gzdsftkoh.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gfdpuijbl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gritiriry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdypwenj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gnoxbcbel.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ggtivczou.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gueyniyvl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gwjywzpaq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gtxglqpdk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gfcsmpybp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/giyfdbmot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ggxsmehrf.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gcpnkyqne.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gufivzwiq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gecmlzwhj.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gwwzkclsj.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmpnhjssk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/golhudcog.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gebiuexik.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gbbgerpli.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gsmsxienu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gydufkuyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gfgablwaq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/govhmwykw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gamrwptlt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gguinphdc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gyxugmjfx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdbnhoesu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxfblqxhp.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/grvkrtevn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcjmuraje.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gqmxrkdpz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gfxmmyorq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gurwfrcxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/grrojdrfq.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gtdkhlher.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gjplvasyf.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gxxwjxlju.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gxidknhfb.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gmtztadcu.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gzgtvbziu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/ghnsmiyzg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/getvpwuts.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gsilhgled.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gittfhaej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gjgulppvr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gsoqwkdln.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gmxcmooka.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gmfcfpvwk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtllswwfi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gddtmejin.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gclokccef.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gyjhratzi.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gmwfgpczw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/glyiyibas.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/grflxugom.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/geszatbrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gevqsejhp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gwqjpihmi.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gwrgjarqq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ghfccqxke.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gezjvuwix.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/guxoddxmh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gefkuvaqc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/ghfledrmh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gsdbqnbuy.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gdkaswuvx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gwwkdjxgk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gxankxmlo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gkprelcaq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxpusdtjv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqvxcujyx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/guurbcxjh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqarembu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gjmfxiyfl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/grrzxwccl.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gjjviouab.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ggtvzxjyu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gfufgqefh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/goreskwle.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbkwwvhri.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gipowngpl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gypdmrwlv.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/groaomhbv.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gfkvycrct.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnlznqxiu.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gsruzdoje.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnnddrnpx.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gzwfmbzzf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gauisqizm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/giivyzcth.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grgasgqte.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkyiyihit.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gtnihhzyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/giiurygmj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gpskjsnis.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/glieqrvos.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/genchyqut.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/guogpobvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/goityetwp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/glmiholdh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gimuqibgf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gmlpeghsd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/geckqstlp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/giitbxpso.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gtihesmzb.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gaarbzbou.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gnexpdcna.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gvuxscfmc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ggidyrdqo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gyjqaukeo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gioezsqxg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gljgvtxst.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/grqbktaen.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gwjjpxhvn.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/grbwkwiat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gkgexseoi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzxwzghyu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/giesrnsfm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gdpuoyzpc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/guwirhjzp.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ggnjzgfdc.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/ghyvazfwh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfckbaiuh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gzjkmlepg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gaftuooav.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gtlswdngi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/grpypujhd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ghtmywrfu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gjtwfbsrd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gzkppniwr.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gmecaqyoz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ganiqjtat.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gnzttmfuc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gyskvtxrl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpcqtupys.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/geryjpbdb.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gyrbsbklu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpupahvbv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgssimq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gapeawlgz.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gaxoxdkni.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gmesnqnam.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gcmqijovm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcmetrggd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gkltakpac.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gocqfbhfn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gqavmkxug.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gagwypxmk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/ghmkqalzr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/guwkvkgwh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gicmkzpnn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gpnmjkbmz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gvlgkaqqp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/geykagrek.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gtslczrkd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gmyzodgdj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gsjgiujvf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzexrkzx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gazrqynrj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyjqixdmp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gwsseeqyn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghkeidula.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gfgbsagmz.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gusggpovn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gbpxcrdmp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gnauzcbuw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/godwugkzn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gohzvedkd.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gqqxfcdyu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gcdnddnct.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/grrngvqhq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gemhstozp.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gowsuyppq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gjwlslkew.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/geacgdbyg.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gaheobhde.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gfyxrenet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ghlfvbmkc.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gmzricqwq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ganrqjbki.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/grnwjvvsb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gccgveajh.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gxvvklgpp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gnnegfvho.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/grtbzcnwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdzvayykf.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gfmnatekb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gubkbnsui.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/ggsgjfjov.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gfywcwxgo.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gouhzqmat.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gvtdcqfti.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gxwalnpzo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/ghczcweqa.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gzzihllaf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gcivktlgm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gqhavible.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwagfofcp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gsdceergo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gvcaatcbp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gejhlnwyd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gyqikwnij.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gdcdfuudu.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpmavxveg.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gvftdullz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkgzylt.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gctvupitn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gymagmtct.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gjrnnrbvk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/goxcywoso.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/ghemsolvt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gwluibsyw.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gqscbopbj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gowccnxkk.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gaoyiotef.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gxtmdakdn.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gewregoml.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/guieghnly.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/ghwpavpbt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gfcxffjkr.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gqwwyfwkx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqdclbzjk.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gqjnxylwn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gskhxsdoi.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gmhutiomh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/glwfaoupc.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gdbjzuhna.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsxgmznpt.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gbdjbfgay.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnyrujyig.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gmwmzeclp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbweiqwdy.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gxzbehecn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmshccmnu.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gioumgobq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gnldfcbiv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gbzcyhpay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gjhzvrniy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gvpmnrblv.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqantxaqq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gxqlpcnob.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gnsljymcc.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gysalxkgu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/goayjdegf.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmpeooneb.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gocwpncwn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gidralbdw.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gmyxqlses.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvhpzpnwd.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gxlgbarhu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gfaeakcwd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/ggmqndlky.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwvpglwfl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/ghleysafy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gepbksaaa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gzjneqseu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ggpqrtkew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gefapuoyn.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gqcldgkkz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gdaziuwbn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/govrynjqr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/guyidektk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/ghwyzogag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gjdvrozdb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gchqkxjaz.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gdlykvkdq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gjonwqebg.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gwpyxabuy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gzsswvivr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gkxhcvufq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gxjcygwqg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/glmnngzis.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gfljvwimv.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gbaspdsig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/grgmaccde.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gkluhgipc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gukdeoisd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/giaygpeiz.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/ggtdiegus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbgyjzwya.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gffqrxsfk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gntatkffm.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ghtxvlhud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzoomkebf.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gglyncqiz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gakhlrhjs.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gjljdgrkd.sHtML


<!-- 参考信息 -->