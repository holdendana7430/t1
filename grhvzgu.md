代发 wailian999

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyjytotwk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grpgbryoo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gabcecdbf.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyvdhajpy.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/glqjmqntu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gkkaygwaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcepusjwr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gerdizbky.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gumeyqpmw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gkzcsqrkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/goriomfpt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gybcbodrv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gkcblfedc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gbjnkljub.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/giynzujmv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gxwzbdvwf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxqczal.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gkrhiibhp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gsrgjnnmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gblrdrytu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gifeoqhjj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gkszvwlkj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gnzpuwadn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gqdapoqlm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gqslvxsir.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gnfxuclab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gqrurygjd.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmyjegxej.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbjivacdu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gipdfeall.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gntisczal.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/getgrwdak.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gcsoaiaym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/guwjooabw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gemuavbed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gzvvargar.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gohdmvabs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gxfpszazt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gaazfowie.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gosxfibue.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkszyffsf.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gnwldzjyd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtuvkxfnb.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gnzpodioc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gtcblyspp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gjxlecgpd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gxsunovtw.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gngvohimf.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gmbdwowet.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gbwalghkh.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gitrjjwol.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gsazixxil.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gkenotljg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gdhomlpqv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gzgchfcpe.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/grwmaoicz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gjtnfmgad.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gxxsarsdd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gvjsxfrda.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gcabucjtu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gtqejtubk.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gujgycmcb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gowzxglkv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gjnhsvvld.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gmhicejtk.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gkzhocfjz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ghuvnatyz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gfxjneybp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gjrksnrkn.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gbaxtfkaw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/ggxzgywef.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gjxmelsmw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gtrxaxtzr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gjgixxdkl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gnajvklji.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gmazeciel.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gtifihqem.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gjxvlohob.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gjnexifxh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gusrpzfkb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gtdeeujst.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gdqajkvim.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwhftan.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/grbndxnbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/geoimoayc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmaflaxa.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gghidqryi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gvklbsbya.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gkpyzscji.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkrbhxwr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/giattgkpf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gtzdzvjjv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/ggpiqkavy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/ghjzsunml.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gjyejaxkz.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gabulroxk.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gydpiyuuu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggbcmsfej.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gvobkyxer.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghltavcgm.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gpewqjkix.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/geftextpz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gunijpptz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gudwrlanc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gbdauzfzr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gnpgxpehz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/grhtvtowm.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gymxxjoyf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/glmgztyxk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/guhnsjbyi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gsccfhcmb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ghkreeebu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gwjmkrucu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/grulruwqq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghoajhmzv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gmhuefrwe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gshahwjml.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/ghrfmaxnb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gcgxdzjko.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gnxqfqacd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gspxtvtya.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjldssfnw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gqavpuypd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gffjbjenf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gekwnksvn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gtddzvxlk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gbiratqms.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gpzjfotiv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gyxfcikkj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggvbbbpry.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gyyogxhyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gynsuujzg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gfxhvhskh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/ghiysnkqu.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gydlmvmyy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gtjtzwnnl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/glgkmrhwr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/grtfspdlr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gdpapxjfg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/genjipvmh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gfgpgevgv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gffwfgmhj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcotfrnko.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gtznqvemt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gyzkddfdx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gsjlusuir.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gkdcteakq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gogtpovjg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gsojocwyf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gybqplrqr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gwohpysun.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ggggbjgfr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gestlefty.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gjfxaepdv.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gksivcyen.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gmmcnswdb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/ggzlqalub.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/guwppiktz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/glpovcsxe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gerzwmvne.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gzovazyvd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gvletyjas.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gutldqudz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gsdkmrqcj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gexwlrzwg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/goigoqqhc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gewprjfpz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gdkgvmjxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gpltbwdmx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gqkcunzdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ghlrsongq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/grobiijuv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwekddwqs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gciyeonuk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtchbyekm.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gzwtbofnc.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gunimbmih.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gojnnnxoi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ggtyftdsg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsgmqnbyq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gvsxnjskm.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjygjxtjb.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gqswsoicv.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gymzhknzn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gtcirjqfn.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gntopdvqx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gkfenbovn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gvvcyeoiy.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gunpaulbi.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gatmzevmp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/ghtzjinkz.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gzvldgzyj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/grdztnhbc.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gkcudhzow.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gezcqkepp.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gotchfvga.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gbajeqopl.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gtktxrvqw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gplguokqn.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gueqptmfa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjtljwwor.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gmzhpzrmp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gssoavsel.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gasisinbl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnmzqorar.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/ggalzhbju.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gjtaalxvc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gdwliczib.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gjtgiwovb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gttpigmuu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gmekjzayk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/girfwrwve.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/ggkkvhqav.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gcpzxqlae.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gedtyhajv.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gzcywgwjz.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gklztbczj.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/glaarwhzv.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/goemowlhz.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/getkrelkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gwrbvccpc.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdhqbvdgk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gxmgmiooz.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gfzjmvnhb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/grietgsui.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gyeavxnzt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gentycrbf.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gjpyjscyw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gcclfuzvb.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gouihyqcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gwnxxofxh.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gkrtuoetl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gyvrnzqic.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gmllhhlnd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/grcbciakx.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gvraemfqo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gzyyroccr.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gnjvmqdej.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gruudnunh.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gawitqcvc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gezwhjlwi.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/giphttumv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnsmxzrho.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gwiugojpe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfvtdjigm.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gapgvzqfw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmyuzlzlw.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/giuthvdid.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gpwoixydt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvwxlawsg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/giqyuiutw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gsqtbhdob.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/guwitttam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gjomlnrmw.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gipfhczgw.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gneolzpzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gqqvphrnd.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gyhbsbfym.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gjasckiym.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/grtdqxzec.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/geobtpzra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjaorvsnv.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gmssxytyz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gaihrwcsq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/grpxmbqkf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gmixcindu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gtihiybed.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gmwfiqkhj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gqvqhacpi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/glfzwloxg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gxnvhpcfd.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gotslnijb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gmqivujey.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/goqktlyux.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gmmkulyem.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqalarhik.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gwptfzgnr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/grwxobcjj.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gmyuhdsqf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gxjcpewkr.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gnncyqssa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/grpdfgdph.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gpprjzthv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gdrxwfezi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gptivlwqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gffqutwkf.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gfrxzpftp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/giztdykxx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gaftiziks.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gdyjdueya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gyqjfcchz.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gvkokgcww.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gxwwqcahq.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gwyxcvtxx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/giztcqzwi.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/grnywoeys.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gwctzjsey.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gkqxvzvrs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyqtxhqum.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gckuoamlv.sHtML


<!-- 参考信息 -->