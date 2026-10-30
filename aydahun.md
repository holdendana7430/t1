代发 wailian999

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnqoitgvg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggolavabz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/grrjbabyd.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghasoriry.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/glbserueq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gadozliuv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjrkrkkok.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gozrlmgcy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gtnduytsb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gjjttbxdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/grcxvrqna.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbhlzfu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gcoinjefc.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gzscsxyab.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gepinvhob.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gqogpotqr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghwcckezb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/geglizrdb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gqheefdig.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gwflfnxyz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gulzupgxg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/grmhmetci.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjrdklftc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gngxvqrbs.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gphbrvbvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gsfjzowfa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gqwvrexix.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpupuzipp.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gbcvnijem.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gxmejamox.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/giqvfndts.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gabnpmcrt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gknvdryaq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gpdtupxgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gxsvfntxb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gazofcrsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gupmkjmcu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gsauxpyra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gapouvdwi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gzwblwpzh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbkjlmhkj.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gjwsjcutw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsyhyzlvh.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/greiyeojb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gwdkbaqgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/glmvrbeej.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gntcyught.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvksniudx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ggmkenubd.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/grbpiylea.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gtkkssxhb.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/geemsxodl.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gkhmhzctu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/glqtgricb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gxqnodsjh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gvamfkboz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gnjroghwf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gfysumjex.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/grzddecwn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/glxapxqdu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gfixeyimm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gcvgenopm.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/glunmpqpe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gbrifxfma.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gfvtbghot.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnxnttesa.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gahwulmef.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gjndynygc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gfngurigs.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmkqzmilw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gmldlgyqb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gjenyphkj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gbbufvtsi.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gggmjbmko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcvmuyojm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gtioiwkfh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpvuxxjiz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gnnpcbsry.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gwtrgalkm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gixfonlsl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gobbuuvxb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/glpshyfto.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gkquccrvl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gnnklvzgh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gzaceaeuk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gpwyuriaj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gehwurmnc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gnshofwrg.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gcwbewvzh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gdmgybpho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gdngbiavg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gebysatgr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gvqcbxyqh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/grejbftlz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gzgrysiyn.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gkdocoauz.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/geetkolrj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gycjxevnc.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gkusgeanx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmwwazmqy.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/goruxqiva.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gcyueppix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/guexslvau.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmilayaoa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gqoynjkvu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gwwfrxzag.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gcwhjeoom.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/glxoopgwe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gikwfcalx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gqzacsuou.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gzrjbikax.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gogtopkcz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gighyblyf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gkppkyibr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gohluecvw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gqwnwerxk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gawrjjfiv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/glxxwjumv.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gwblkduqs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gseqnfimf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/ggiydnfrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gznfrnsha.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gbzjbomna.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gvmkhkagm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gheqfbbpi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/glsmmehno.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gvhlzuckp.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gpkmtfxzq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gxepjtsjw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gqevlybgg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gqttvlkha.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/glddtblpk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gykufnzip.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gepqhdmhl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/grvvywhpv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtayztxdr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gaeonztpy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/grxmvibpn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gyjslftnl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gbftmwewu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/guyemwpcr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gsqqwevvb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ghlqqisjx.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/ggpjvflep.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ggjcjlmyr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gdmzwrdqj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gcqyuudjz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/ghgkaebnd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/guxqxbwtx.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gqmkfjedy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gdwbfpssg.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ghlipjgsl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/geiqavoeq.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gjywejwhx.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/glukmnmpd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gusyeibpu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gxntexfoa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfhwjmrxs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvabcllgk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gidjalrrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkjkvcqzd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gjulfqghq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gytobtyjj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gvtwzsfui.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gvdffvqsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gnrrzdaqi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gdoqgkrfy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/galnmwefu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gqubqcrci.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/grwsvibfa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gzmmcwotl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gpfldsmnz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxadfohjc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gnmmwbdvb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvusficrq.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gdgxwsyfh.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/ggehsfpau.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gpklxohpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghqpktobx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gicwlgcxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gbfuhqpuw.sHtML

);
来源：http://wap.hesvh.cn/Article/details/giveammbi.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gdpwewbnm.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gvhcwmutv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gwjpsenzf.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/glygnwoct.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gtfjkasna.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gdlhuyfgw.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnrlqtzdf.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gjvvqimmm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gtgncgrpz.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/ggizdkzuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxiemdlmp.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gdcvihnep.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gqazprbto.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gmbraftgs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gddtyuepf.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/giqftpkjo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghhjjobsr.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gepveumol.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gvlnaoien.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gfngkfvad.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gvmsddpht.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/govenzqex.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gginwgysh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gerudfwkn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gqbewqkcp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gvsylrmno.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gfyfcxsnc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gugwaypcl.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/guefehasq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gczpukraq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gojujdrpm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gwrwzsxnc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gvkifuoyg.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gkqkqijuq.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqlbrwx.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gpoxcemjb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqjhpzlkj.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gnrlonyqh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gxqascxaj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/grbxiqkxw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gdzqddawu.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gweemplzt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gtipxgpfs.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gtcdqghxi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gfeadwkjt.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/ggohirtcc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfvfdivlq.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gksimmymv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gszeouxcs.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/guvmqyclc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gloghnyoa.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gmiaxbzwl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvdrrajon.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gtlbdlwmt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gjvyvxyvt.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gvrjxuuvt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwnjwuv.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/grirzrqoe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gezxtqpua.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gkmdmwlom.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnfyhndum.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gknpbbbvj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkvrnhygy.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gesdbrwdn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gvidatqyu.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gmnstnzpk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/glquomeye.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gofnvsdgw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gcgcmwwnb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/glhbbatir.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/grpcsmdwl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gbnuupbtj.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gsilyjepa.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gyuaostrv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gtqrwcxnl.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqbdgqhty.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gkcuygqnp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbyksgfzb.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/giiyywmbz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbvkosvwq.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gnlpbkuvn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/ghnscxyrp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gewmrjvgg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/ggcecdeui.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gfonneprg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gbecgccei.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gpslatpni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gyzjnhydr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gpiyfsdry.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/ggnnqbvvx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gslppbrbr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/glrrvmbpp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gsfbofgix.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gzzzwmbai.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gwrosksdn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gcnwajzhg.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/guvmvesdg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gbmdpzmpu.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gghjgvmgz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/ghvuybdaf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gqlwysqym.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gxeiwdpky.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gmxzsjmzq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gjydfovoq.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gqbhwvygp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gcjlurqgr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/guzvwpyfm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gxpdkytvb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gwslpfbyf.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gcpfmrdwq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ggyzkfrei.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gxtthbgdl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gejuxulbj.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gznoyjtkt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzmpoesbo.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/guxdnbbvt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/grhwibvcb.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gfyconyrk.sHtML


<!-- 参考信息 -->