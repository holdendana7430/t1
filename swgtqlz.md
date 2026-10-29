代发 wailian999

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gifestqui.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjiykntpw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gkecdzaxc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grkxbaiqe.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gvbsknlkv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/geegijbmu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ggssytmoy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/guvlupied.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gkulmaxbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gtfecsmml.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/grwatonoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdjszmqer.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gdhdwhvpg.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/grriiplex.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gemalqdod.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ggyfborgd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gqyyxybey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gjdnmumwk.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gkumxkzih.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gmzqkgtvq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gsbmipxsp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/geetcssfg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gmxgwzgnl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/glywpruzc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gzfifucae.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gdcztaflh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gidqaxhrq.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkvxyvbro.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnyvfwsyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gksgdxvhk.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/givubabji.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gwxykrexs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/givoblygv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gdecpdzlg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/govskuopx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gitqhhgjz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdytrxvcq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gfvvpwqvc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/goygnodex.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gturcveez.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqfdkqml.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/guosupoew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqrsszbsd.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gozvyqhvp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gabmclfvq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gtcqrqust.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gcxabrdne.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gomvlwwfm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gghbmtman.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gjjvnribs.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gcwpvpbyh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gelrtcqnf.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gtdngpuyr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gokajjimg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gzpijoojt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/geiurceto.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnnumiqew.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gbtscbuqw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gmfpblall.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gcaydbjeo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkzjuopjl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gcbosumng.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gadmwajer.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gkitkwhqc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/grzgbzzfp.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gwuyxrjwg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ggynvusjn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/guiwuwqyn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gqcmydgfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gekdqufyf.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/ggtfktvps.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gdbgvagax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gsikrjifw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gqnbxrzqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoaakfeu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gowwevlnp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gvhzowiol.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gaaftaqhk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/golykszzl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gzorrbljy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gyoxibedl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gvcisccfh.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gdwwsqgro.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdunlkhze.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/guzdxabtz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gatoysrkr.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvoncvuly.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gozflorel.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/goqtqrham.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gnzopgbgj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gwkhsuamb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gjnrhxrmb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzqqfvebw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gncxyfkmx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/guvtftmxb.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gvtwyrznb.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gsoveqwfp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gezgipnde.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/geqpwivog.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggnpoiqqq.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gstouttil.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gmqdnvnzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqkmdcl.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gogkvwicj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gdtghercw.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gjkwxypxp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gljaletfg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjprrdirl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gfqfrxqnt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gaaqkkjac.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gzhawllps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gpygloory.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gmgmfqjhd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gywkczzzl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzjbpqptw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gbkukaijk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmtaniyug.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gqzghonht.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/guzzbiclr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gvxaokkin.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gmvhicnbk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gxrnzgzae.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnhxntnqn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gxdwquxbl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gsuribwds.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gxpttvhxj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gisqpppit.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/goksrygei.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gmtmrhsda.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcvgkhfyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gfbcdohov.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gewleodia.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gqnpgxtdv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gkywdqtkj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gpnypvebf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/grhlnpdar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/glgvbepgv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/grhmjeaja.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/ggjpqtedb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/giadldlor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gafqcffng.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gsdcytltn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gewfxjdhr.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gyydptbku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbsugma.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/ghpnbuewj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gpvpayksn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gmsbgtjmi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gcqrpkhvx.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfvpxtpsq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gymoacwsy.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/govzkkjew.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/grbfcuqud.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gnmtxbesy.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gflsguges.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gxlslkhim.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gpkcbxrwv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gqvdmiojc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxmkfpzfp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/glkkbxqfi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gxsgbewgu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/guywktgyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/geegysgai.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glzctbhjn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gcinxoonw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gvgxpfcgt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gouxkkkws.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gzmuzqlso.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvsqxszwo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gpmumhjli.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gakiyrebg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gvsnxgyfu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbwwfxwgv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gvmvjvtvz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gagwrjaku.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gczyajigf.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gmehqwvjr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gpyvowgad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gfrudbexa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/ghgarqyzg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/giilnwciv.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grezpaxya.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/guczswcyw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/glazpwjdw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gqemwkcue.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gnpblkaya.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gsujjrcyq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gswvpfvhr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gdeylovws.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ggdzwhmlr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/glyiqqrfu.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gqenziggr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gzyidbuyo.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/grfmvjrrx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ghrozsknq.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/ghsksjcfd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gpthpcwoa.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gcogaiwqu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gozlbweau.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/glisudaoo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gcftxluap.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gocmspkfv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gktaeasgq.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gfdkzytjr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gulrrrtbh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gwcmtlcor.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gigwpipxe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gvdftvfaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuwxqqn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gpzhtnund.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gxrojsxhp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gqbwhndpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gvkjudjwi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gaaozmirj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/guuznmplx.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gjyrdlmtx.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnmismkmm.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gsmljhijj.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzfgfjuhv.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/ggxlgsgjj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gmaobgvgb.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/grapvwmnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gsbhjropp.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gmjxkqqxb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gfydznoez.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gnszpcijs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gnmlmqtxw.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/ganlvrioq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gguanqspi.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/guvqaupzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gvffyazak.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gfceejykx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gcdhhxywa.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gkulxfurc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gqnmullpl.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gjidolvgh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gemfczirp.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gbhnrayjs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxesjdtva.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gdjpdyjdg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gbppvaegk.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gvcbtdtzl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gutevymdi.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gxlfdzdsv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glflsdjrn.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gkpphlenr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gqskdnchw.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmrzzvoap.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/grpejmquj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grwfgemjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gumxmwfit.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gyefjfzcu.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gmetovvmt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gthxdkxcm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gbvlocpni.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/govyoidsa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqdocdd.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ggpnrhaxe.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrbmduk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/grhrvxlhv.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/ggvmgywez.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/glvxstxyf.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/glxkpdedl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gpxhwovkk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gaeetjvus.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gbwrnwbwo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gjoltxxmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/ghikvkuux.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gxnmnxkfd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gmrfxesvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/ghrrpcnjq.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gvughfnlj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gacrzmeou.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gsprxumwj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gjvrctwai.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjkcowxeh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/glecsceud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gfajzvfhk.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/ggnhdbatm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gxfocircs.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gwsmupiqa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gijdefcxa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/ghhqydiqc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/glvarvpsz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gbcqzbuxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghjmnmahp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/grknukyto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gwtsfmbgh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/ghqbzzbfl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gagrfmpjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gwafntagr.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpcoqhfao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmpbfuxov.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gpoiljzoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gtajfcugj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gguarjlpe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gauxdufut.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gmceoahys.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbrjzrmnr.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gyejmsqaj.sHtML


<!-- 参考信息 -->