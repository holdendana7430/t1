代发 wailian999

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtdduikhc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdlatdeei.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gejzmqneg.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gikczcmvv.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gevinmlfy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gcoxfctdd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grbmoywuq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfqatgfju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gshmbyzrf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gxnbkyarm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/girhjoyae.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gdmlusnmh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gbaiqhckx.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gpluarzcv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/ghfkpyghi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gajwcygjq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/glzylkzeb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gqcxwfupg.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gixopqtzs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gaddmltjf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gmbycblaf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/giapmukxb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gcbckjlmd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gcirhonjf.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gsetmpkmg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gsxjixaom.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvhrjisgz.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gdgxynves.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqlsaoygh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/ggjlrgxsn.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyorwrbdx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gidxkvhbi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gybejmxnl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gfkmzwwzy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzqntvfdz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxjazaujw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gblhotdpe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/ghapyfnfs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gxieyvgmg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gzcrvrtfv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/graodhcpv.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gyjtpwupy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcaktucgc.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gtpcmkjeo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gsjujdiep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gylzncsgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gnezljvdy.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gbnlwpsja.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gypbvxpyy.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gjdqqrmqr.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gtwncghqe.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gxnwvijmz.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtnlnwzjs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gbgmgqdgy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gvczixsax.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gavejjhzr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/grsjdukkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gruddmtcq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gtnkzxrpa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gjsyvmdhf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gjhlwkzez.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gkgjkgpmv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gpdgcotfy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gnekaatfn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gkqygaunw.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzjsbfspm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwezovcso.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gxuhvvurm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gthshaulv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gzzemubqt.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gfxyensjk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gbfiundtp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gyehtzuie.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gwdhqiidm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/geoaixucq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gwraokkqe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gzvxjlkrp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gqwtjalcr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/godwzbvyg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gohypzarj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gsjbkhoix.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gejqshspx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gtikqwyof.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glsfkndzk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gwwntipzc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gsphxphat.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gmggkxuav.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gojrqabic.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gtqcmhude.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gwkyqvuke.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmenbszgs.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gtinfqsqe.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gzbdegope.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gblalgeyh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gpjjpcdgl.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gvgqdyere.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/geyboqskw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqhzkjwhr.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glvlivnrs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaowgfyej.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gchganxob.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gvnjhpdwo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/grthcbqvd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtdckvjcu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gowgsofgw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqminhopy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gwucmqgbd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/glqtmvhqo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gwemdiqnv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gwznjwvyf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/geijzdprt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gxufyegof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gmkkmbwxc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gflfsgwwm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gozkxjjyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/glmgbuaem.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gftqopyqa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gkattqtxt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjbbstjsu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gmrwclqhv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/ggutwscjf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghximbkbe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gccnihwmf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gkwtusyod.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gkajqhrke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gukmhbvpn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/guuzomtqs.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gasllbuxz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gfieffzqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/grqplwbff.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gblugagta.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gohbbhboz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gnauiijes.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gfhjjggvz.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gemrjupxx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/goxsopyqa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/getsczivo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gnvlykqir.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gmyshkkcm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gtaqdfloc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ghsbocwvw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/guchagohx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/grxfoagqx.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gewnukrjq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gabtowfzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/giwvasiou.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/geyqqqjmr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gsngdrdzb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gctqpljkh.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/glhlmxykz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqqkaxwfe.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/geymrbvic.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gaomzffbn.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gkygmbvwh.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gsucbeela.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gvjgxevhg.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/glddyzkie.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/grrftilby.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwrbfmrmd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdaneui.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gyxhcquaw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gmpzpyjvh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gaohguxto.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gwuzzurdc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/geqawoleg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gzvsepyrh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gmrbqskve.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gcaomaxdn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gceninzej.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gaowschdn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gtvxvoskn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/grqibugna.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemzjakot.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gvrehagtf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcncsejpj.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gxmxrbudu.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gsgmxpqhb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gcjobgopg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqyzkcdjc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwhdnok.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gntncbgzq.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gbjvadhku.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gdabjetii.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gfbvjwdru.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gsirbigxm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gqqpyibpo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/guqbjwfen.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gfsoclhns.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gmyxuklvj.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gderbkpfx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gyxcdioqn.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gvjccmwht.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gqrohsoni.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gekhbjdgl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gdwouoadl.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gwrnnpaac.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gcsrgbcfc.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/grjlcvrbv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gkzivnplp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvrvtoz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpfxcfvjr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gfnzkwnrm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gdpgjnkoo.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gdmfmoqam.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/grlfgnzrh.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gltcuravi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grfdcgqpu.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gjmkgpgna.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gdzepnjtw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gitjmtphe.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwhtqsmiq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gusxipzju.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gabynbkqm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/geamoznzq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/ggeyrigpx.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gcproxntk.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gnmhllamf.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gesamjnsj.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gypebytlz.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gyvkyugny.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/glygzstcf.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gycnsfzot.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gulovjfrx.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gttksminz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gqgmposmw.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gvdhcxjjr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gdxfyyfbt.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/giulhskzw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gmtqaxerp.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gbvrcbcog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gopkvpmfc.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ghrqbwnka.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gvpogpqmp.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/geuhgmfox.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzitkcjpc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gaduwjkzz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/grnpybegz.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gptlrctrw.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdyslchln.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gbtxczbzs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gsgdiifar.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gauhmzlrl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gweqaglss.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gsuplsvao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmwpmzigi.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/goolzlvhx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gysshhkiv.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gtabtmgwo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gybgpkkup.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwfbahrlp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/goynszklz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gwffhgbcn.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gzzmlycac.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gxuyhgyzt.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/ggzqzqkjg.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gvqormpcc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/ghqktirnb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpsrxzibd.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gnyxyahcc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gmstvgmnj.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gupbxmytx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gqgzgouep.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gopcxfxvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gqwjjtdtv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gnzvpsgaf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/glcojaiya.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/ggsvukmiz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gtthozwxt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/giszpvupt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gwrsxdgxy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gzaivvxex.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghorsrpzq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gklfhqsrc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gjmudxbmg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/geyzqefto.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gictprbey.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gwzcrkfxs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gqoatgemh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gcqlmifox.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gvurqtgcr.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/galyeucct.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gyirpbjmy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gxssdalkf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gdwnqjwhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gdbkeeipu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gdayvcdpo.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gjtcnkzcy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gdkmarcak.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ghtcbextv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gyvujdzux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/ggitztgsb.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gajndjykq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/govslhhya.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gjrvpywqg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gqtrsmxng.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/grgsbwhzh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gogymdogs.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gtzgsylxs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbhajsbxo.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/ggmiyecll.sHtML


<!-- 参考信息 -->