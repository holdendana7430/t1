代发 wailian999

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gpetymdlc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gttlxxycq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpjdelwio.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzlaomdiu.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnwnnlqla.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyxagdcoi.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjyxksuhg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbxrjrswu.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gmpbwyiix.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmqcyujbe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gunldplnv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gxfqxjkla.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gbqlvoabq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/glbsksvrz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gdkehqazw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gstdimvul.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gvhvnlwib.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gjwgbbwfn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gzpisipcf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gzullsnpk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gdxomrybu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gbshmybdc.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gxmqgogxw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gbhuwaccd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gzjypmyjd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxwgyaqs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gedzvwzmi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gcogazzpq.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gjbpkeqzr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/geqibbfio.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gxdixxndw.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gnjzukdlm.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqmiqqyox.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gamttofwb.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqsghvlgy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gdjhfdysk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gcwuniqwk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gqjoaaydj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmjpyxaaz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjouyiwdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gvnmgggqv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/grqxjdmen.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gxdtbhbfa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjzjiumjw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsujppvyw.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gwnqklyaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwrdjzvud.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ghcrnifca.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gvbtsilyz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/ghvorjthh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gvqxivxvb.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmacdtwem.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gwucjcmda.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gdfaxuxsj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gqfebltwg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gewhzxbtn.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gamgdlsuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gfldgqafb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gfjoywatl.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxoqtfftc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/glqockkkm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gnvlfrtyk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/grroapwmy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gmtdywrfz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/grhigyljs.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gkuqwwlux.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gkgclrdoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/ggbyjtlzh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gdtxsrdzs.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gquqdwcjg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gslfcxbbh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gevnestlc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gselcvwva.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtgozcalg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gzjhljhge.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gagdtciej.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gnferayqr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/grvltrofo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gddchjlpb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gwovjggfa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/ggffxfhtd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gawbrhyqu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gzuuzvyxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gifzaclgo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gfbffpnav.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gvipjrmqa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gwxyjxmnz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiqmtss.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gbyvzyemr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gefntdyva.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gojuyzmfg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/glulftfqf.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gurjcfxxi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gwaauapel.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gypfyntxj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gpgjqomrr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnnlcsrwz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gdlsktvpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gbvbruuwq.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gtyvveypr.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gwuzcwaiu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtqkbvhgs.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gmaxelqhv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gowunqsce.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/geaydvttv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gdkeomlih.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gisgkpvtb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gllylitja.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gqaldgboy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/goqhljeti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gkejqvotl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gvofitxir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gvzkjfrzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdohpopao.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gbmwnvxyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gtxdkbdvo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gppmzqqhm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gqyirvfre.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ggrsradnu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gdqtijdus.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gfqewoxzr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/ggpsqpzth.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gidwctgrb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gmysuuxwv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gibpwsclm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvtzrydpl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ghcocmeoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/grloenjlt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/guujjhnix.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gozmvwrqp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/guyoupyky.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gffhgikjw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gxwylyvag.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gorgucout.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gozfslkqm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gniadipsx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gtmmhncsu.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gkgaaavkh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gxssrzlpm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gzlzcnkep.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnfyuqfrd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ggbimrgtg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/giizlaeyq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gbiabkwnh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gkdopzewr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gzsghdkvm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gzmmoteww.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gtipczmoe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gxujrqgfg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gejhlydzh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ggwnhahcx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnavlzwhg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gtjczmpgo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkcvjbouy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvblddqyg.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gbpdfnwcp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/ghfluywad.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gsmcqesub.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gtovhpucl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/goldudzcl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gbxnaqeps.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghcupqdah.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzymncoej.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gbhkgdhxo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gnsuqverv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/goxwcuwrj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gibzzghde.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gdiubpmbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/grkghuzbl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/ggrukheiv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/ghvxwqmcy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gjcobrdwm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/glwbnuryn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gcepctkku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gpvvhwvyf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gwzlmleam.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glrtkjopt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gentcjchu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrukovbf.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gyftapubf.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gfadndtlw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gfplohbgc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmfnprfdv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gytjvehnx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gzlmrqjzh.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gthcdcggo.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/grtakshih.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/grpvjdhjq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/glvafpuoo.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/glycyivpk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gvbkwhunx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gmhknidka.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqpurxsta.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gjwnmkddk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gmgtfftnh.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gyckzlatg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/ggvmqaznw.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gonvmivwx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gwmxgvxtk.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/ghznmojua.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gvnjnrxcr.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/genapphsp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/guqfkkruh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gnzyjfere.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gepjcnqtc.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gbrvqmjsk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gcrdhjhuv.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gggggnyro.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gmvsxqflo.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gkzloukwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqvwqfeaj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gldmotqsp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/giftcetbb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gpaxhcmux.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gbsbiiihg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpmswydik.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gwnbndfma.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gqrpjltjb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gzoujqnlq.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gchebfbub.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzqlbwhro.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/guzflifib.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkcfhlcpz.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcxwifcwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqttskvnc.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gbrxvvubh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gnaonzyeh.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/giwnvihqn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gbpaqdvsr.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gaoudexhw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gullsvjzh.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gypjpsbyg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gtcdonhcg.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gndwlqysc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrttwlqn.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/ghepobplm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/grhqjxgyo.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gofgmtodr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gevmvokpk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gedmtgabh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gqchuinwp.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gywogdekf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfpdpitvx.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gmadvlyue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golxbqftt.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gtkyxxbrf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkqhzqomh.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gdeeiwzwh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtkdnkder.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gjfmdiimi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gllbdwosr.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/grsuzhyll.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gdsosznoc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gntzkzzvl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwqeledgz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gnssflvom.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/goscrclhb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gykcpoove.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gnqzkaajo.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gdsgglzqu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gexnvydjr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwocttdtn.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gbqshrxbo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/geikojfhl.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gtojwtybv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gipcxqvyf.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/guahrrcuf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gannxprko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/goauajpga.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/guhugvxxs.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gdfsoimni.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsnahlq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/grqhbzusf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gmkjkyjqf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gceimbmbx.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gjfnlespm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gfptkxehg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gvetuckpc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/grtevnvnt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzuitjzem.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/grwzdoggl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/geomarcfe.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmgrihwjm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/grkhbicov.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gqxgtklvi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gyeaqdbbz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/guwrcpysu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/greuatxsh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gohshxuqf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/grihclcmx.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/getbilede.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/geholvytb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gnoidwgpf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gszidbeha.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gqgeijykz.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gwgnurgax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ggfdcbyln.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gxxeygzzj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gnhparnbo.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gjavhqnra.sHtML


<!-- 参考信息 -->