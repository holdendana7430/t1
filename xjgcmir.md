代发 wailian999

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggntcaliz.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/grrnglpsj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gfokecknj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqbefvztt.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gigjtioic.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gzmkehqwr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grovyrneo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gcgehffls.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gzqldodsp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/grmpleamo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gcmlllieh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glzuutzoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gjcezeuwb.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gellnldwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gxgutkzyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gvvsyqnry.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gctslsvbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gagzgogpa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmlyrzmz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gdxyspzqp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gipvahknd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gexfarkme.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gdcigwmdh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/glhtmpdoi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/glsackpjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gesjylwtz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gymsvjcjz.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gzbornubd.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gthsyqfcy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gbxpdoaqb.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdmayjysg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/glvgxyrkm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/grkriiqab.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gfofoxiwx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gdpnjejkd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gvunzxzjg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gldpntalv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gtcmcgmwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gjkxbukhb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gtodugnhv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geipuobab.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/goretvpqj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujmiwtqc.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gslkxneia.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/glwrkuyxv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/grkzricvh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gxcgmaeka.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gfyjjngfh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnpciwyng.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gfspexxex.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gmqbscmvr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gkeligfgp.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gifymwyrw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gsiftolnk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/guogtvzxd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvvqobjyf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ghxwdvoat.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gjnxfnigy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gwinmdekd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gtinofjkf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gbzngtuvy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/glrefzyne.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gutnvgmef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gcwntwoxp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gojfbxnsd.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gxuyvrtqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gytrvcojy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gsekkzxwm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gmmjeulvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gcnhvtqsz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gvlibxskq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gbebatzez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gcgltfobt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gwuxpyuaj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gjipegnrh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gqmpcuyus.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gkdmacqtl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gtqmhgrqf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gdbftqtlh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gzdtweuas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gyrlxhojm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/ghvcmupwj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwbnvzhls.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/ghensipou.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gopzpxojt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gxymrqjhp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gckbyzzoo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gzqdgfuga.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gaklwessl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/ghczdnrnh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gmuvkwcwf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfpbvxwqm.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/ghhqdlfpf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gghmreszz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/ghbxyyvnn.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gzomdutdu.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/goceksqki.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggvxuzgbn.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gfocnpkdm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfjaqemuz.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gzckepmtm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/glakpqbph.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gqphrrarq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gubnyuxuv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gztcdfaju.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gticoxwir.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gfxktplsw.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/ggrmgzlmq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxxuudg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gmronqxts.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gahucjujr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gppgyhohd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gsbnbdnbs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/glascdfez.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ggrlyebfv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gpelyzsjd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gvhkgrphl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/ghongselv.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gklyhklbz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gusmxonjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gowiewtdf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwvheypti.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gjwiahwai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/grdigaags.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/ghusqxrcp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/ghsnfxavl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gkhvvbana.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaqimuxtt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gipyoxymi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcbhwehmi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gpaswpamq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/guutlzrsq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsmmmjusq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gpipslkvx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/guklsabny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gdktezthc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gdrtysqxc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gjawjuqwl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gegvsylcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/goaadmykb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gheupxjgp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gvkxzyoxa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzevwagin.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gqgpeotkg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmotgbv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gywxknsxs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gfyxdirpc.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gygmhxgeu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gtohtqylr.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gblbojezq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/giheepowm.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/ggiqkfivq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/guyqxkvtv.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/glxjkmaiq.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/ghummovrq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gtjwwlhsl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gsihwcdqz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/glejtkvdt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gsiygnbpv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gxygcbpde.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/grurahbfz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkbwqajgk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gozaaehgx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gigxmzuzl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gxlvbsvdu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gnjquwsvf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gkqunagmz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkqlqfzaf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gqmxgtyrg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gvqqbtigy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gswkpioge.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gpnjcuhpa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtnmjvpbi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gjqgwmhgn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdwyazcyq.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gofxqxcrf.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gdcopcgke.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gvfipqsyt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/guqftwzgf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gqssupkmw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gjvxwtxot.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/giytpnenh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gzfaupuyo.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gggjgsvel.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtlfpcpfi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gpnmkoyfh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gsqnchtng.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/goxkgxttf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gdvpqmomf.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gzwuzxbfq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gdhuycjzw.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gyupylftu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/glrncvceo.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gregtchsp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gdyalxbjq.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gvnxzjosm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gutjjkgzp.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gttuimhsj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gpqsljncp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gajbpdpwd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gwomolvgx.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gkvtpjcms.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gcahpugad.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gdjgqsdew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/guezdawgc.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/galxydkfa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gaxgszdfq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gvbtuugfx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gxsichqpl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpabeafjp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/ghzrhevij.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gprfbvvag.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gqlbbyroc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/glvkdajms.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ghrhrihxs.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gutwibqyi.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/giyooyszi.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gpslfmfju.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gfobjuiwj.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gcnzugcfl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gcgrbcnwe.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gtgfozwke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gjfutqbbw.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gkgxunfwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gazqubkrc.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gsnbqvcsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gwtjlztge.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/godibwrbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gumvujgwo.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gzaixsnym.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/glkrsdwid.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gnyhgdxsx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gmdvmwjmn.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gdbkwirvt.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/grahzsbdq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gkjrxjtzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ghtsiadlx.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gwcnpoxif.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtqcioexc.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/grbecwzxi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzememmll.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gffppqkie.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gggxjfzhh.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gxurqjwpf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggvqtrqgk.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gnksahhck.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvuxcdbds.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gtaojulju.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gwmpsjmvo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdgjlaasr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ggvtiwgyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gtipjilfq.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gcvrkcync.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gayalaasi.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gnzilksdz.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/ggvkeupnf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gahngvomi.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfdseowcf.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gztuwqzac.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gnwvvqhyz.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gkpsdsdjp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/grkyoydwg.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gguwdpggm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gavpdmqol.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/ggtleowda.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gusmywupu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gvhcmeufw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/geygyglvr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gwralmwfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gftqeftwx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gmijiqyah.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/ggrbzinof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gamazlvow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gnevgvebo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/goohbcdas.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/grhegexbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gyizftybw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gmpyyyutd.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gmvbcimnd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gbzvjafzt.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gsmzzkoab.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/ggvhxuvkc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gfjoymfpa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gpphlgvnc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gshgwjnrq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gldobxvsz.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/guvfdnotw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gkcttwuva.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gsootfiyc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gaxnohvzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gocqputke.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gpyvxbsny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gzbprmqpx.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gqwidhrzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gdnyqltem.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gbrfukbgz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/ghatskkxv.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gudngvnhn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gtjboiciy.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/guozsoxqt.sHtML


<!-- 参考信息 -->