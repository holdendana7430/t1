代发 wailian999

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnfbqqyfb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gibkgdgwp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gdzfcthpv.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gggufpyja.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gfmjdwsso.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gcottuzfs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/goqthmojn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqarwzdkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/giskzsfgb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/ggvuenezr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gwkfzyuyt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gdygxioil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gualmbgfq.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gjetxxccx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gitroogdi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gxxtrqlra.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gskgfajmi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gudekohlr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gbnmpnaav.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gjtlfttik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gvpqqpeyh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gycofeqxq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gklimvikm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gvdyslqli.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/guuiflkbr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/grkrzhizj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/glylhmpeg.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjxbkwiqf.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gclvjdkch.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gmxcdtrlw.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gelrtsjql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gwtpwvtml.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gdzibnmpk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gkeethnlo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gtputwrzm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/guniotsvv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdfjdwquu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gwxghlhbb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gjlbtkjps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/grovxwvnh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwiabuxxd.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gfugicuiz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpphklqvy.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gdzhxalcc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwujnmsdk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gawmoetic.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gmdohuijs.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grfufablr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gxurmkpss.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gllsexxbh.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gfivzypgo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gncibddqa.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gsvulzutg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gjwbpeexy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gnarhsfrt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gvxbrcbxw.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzzsrxsoh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gzwdenixs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/glhbsuddq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gmarquhbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gsxdamskn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/glkpryzdc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gnnwbyilr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gkxhpmquk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gaybwzzmz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ggjuvruwq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gugurrvna.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gvzxfmqrh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gikgqbduf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwurniqtn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gthjssgpz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gampsfsuf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gtownebbz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gdrvnqkvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfvmdsruz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gtunttwwe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/guzuqekah.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gxrdrttcf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gzrzpxvcg.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gnmlbpcid.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gahozlfln.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/goebjjgqi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gnogdrsek.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gpthmfgfr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/godmborkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/geuzyhuhv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ghwsdikxf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gcvxcnzoc.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gmszredha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gdpdjvevp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gxgzmgybz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gfttkqrpz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gvvqwdjtk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gvgkmblmz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gtguoihim.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/ghxdhvocn.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gxijixfhr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gautzubry.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbpamanbk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnznztuva.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gumfgshzh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gvclcdeec.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gvasttbll.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmlgztqll.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gddnhghbv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gsatrxhdk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/galhseskv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gwbeebkuh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gquttliou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gvqlroltx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gwojsesva.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gtzntazjf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbrqoot.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gafvlekgh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/ggaspqgpn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/goxishveu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/glbootdzj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gdzpcpxqs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtyceqboe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gasxljyhe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/grcfyllks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gaentzijg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gdjslmlas.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/glzvlgrxf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gyelvadot.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gpwzknury.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gyeiihipb.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/grtjnchwj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gopphuyil.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtzwallno.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gbyoscdmf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gyslgutnz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gjhsttdpc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gedmnysrt.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gdxuiztof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/ghotnmptb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gjvwgbihn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ghgquqili.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gwlopgvai.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gcuyulqml.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gstffympa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbkwhhrzg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/geiwkodbi.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gtfsbuwku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gfpemfwij.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gbapqjcbm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gmrrdkvoc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gafhskuex.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/ghyyzwstv.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gkgmchzxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gcuacoppu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfipsve.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gaqpflzfg.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gjsgisxdn.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/ginrqzgxo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gfdpqivlh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gamzugnag.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gxkincdee.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gjxkfhttx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gvgsxcyis.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gdcclvafu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gohwqnnud.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gipwzzsis.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/guaegqfsw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gidfkaqvz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gcqynpisq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gwcxmbjer.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqudrtivf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gqjkfrhtl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/ghjpumyod.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/ghhspqjpr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdjvrtlsm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goqcgpkfd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gctcwvsdp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnnmibjcd.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gylkzutqo.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gvfevxisz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyzuoedqw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gvttlqibk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gblmpyfjv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gxtchlvug.sHtML

);
来源：http://3g.fehbvm.com/Article/details/geqzdutxi.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/ghbtrogse.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gfrwgoplu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gzbetdhwd.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gndwfxtdl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gyhuzampg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gsejycpid.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gtdbringy.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gibykosfw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gnvxupinm.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gphgkzpsy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ghoxcqhko.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ghyzvhvup.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gxrxkvsiy.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gucsfnurq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gaxeenvcr.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gnbelfgwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gpvjuchnn.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gqwilffbb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gatniipvz.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gmxafrxyf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gsmbctuzo.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gpvcabvla.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gudgzlydg.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gpsuqfutf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gjjelokad.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/goktlgszi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gcoyfhmkb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gknpddndz.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gmkcskqya.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gitqcoukq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gbsgzfwvx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gxrwjnglf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gziptlipz.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/ggfxtawib.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdgwehuyb.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gvyzcvtxd.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkskebaoo.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gajtjuzod.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcjhhtdnt.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gpntrdnoo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gehwycqep.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gykcydnxu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gjniupqhs.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gdsdduofs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gblbmolcn.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gntlbhiba.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/geviaitwr.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqesfwhoi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gpgmrsjak.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/golbxxmhd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gzcoqjhrn.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gkpiddury.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gidyrxqrk.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gojxgxypv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gwmhymfqk.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gnmrwqpfc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggjvxmfhe.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gmzdyqqof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmubmwngb.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gmpxgwfoh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmtizshbr.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gmbhtwcjv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcwmogeyj.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gutafcdrx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gksldbmpa.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/glvcpadpv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gbjzyrxke.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjagbekyw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/giieelzlq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gtsqhktdk.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmiuegikw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gqgofchfw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gosuvtdkf.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gmuxigexj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gbkftxftl.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gcezyhuoo.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/ggnbvatkp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjkvudhxy.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gjejumyfd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/glvsolraj.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gdwycgnnk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/grpqpilop.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gvqdysrqu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gpdwzypeu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gfgotmkht.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gncpehdxg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gedwhuzls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/grgyzldja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gcmcqzpjn.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gvzqsqnni.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gcscerbgj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/ghpcppcvh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/geeqgfcrf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/grqvpnabx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gmvhcgpnv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gbrxjbtkv.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gilkvlske.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/grjhupetx.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gxxomabkq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gyldyucis.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/guymappeb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gpzxrchtv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gdvqnyjys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gimsydmez.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gjwlbnmmp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gnzyacdvs.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gecbupjdi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gukuigiii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gqiwxjihs.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gawsrmqjb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzojukpae.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gyzheiina.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzpndjiwb.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gxfkcmdoc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gpnaegzom.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gmdwfnkzp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcesxhva.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gukkoeyuk.sHtML


<!-- 参考信息 -->