代发 wailian999

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gsvjyszfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gswlexdax.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpeuxlbxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gyfpnhsxh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/glfhbgfps.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gjzfebsip.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gnqnjzsvg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gpubkodyn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnymfdqys.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/giibsqovi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gnnogsmfp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gotclqdvk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gdbhesahi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gwqtxtgco.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gejhmngow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gystasymk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/geblwkbih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/glnmbdvsy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gelmqifgk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gtgofihqx.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/ggdxkzjsw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gcvafgadc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gkzyejzwd.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/glfubtxsy.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggyxvgwyi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gcxfhdmfe.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdvneehuv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gwwmradit.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gdtambtzb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gxnzzqbyc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glatqlazd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gokrhpkgl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gewonpkfv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gfpmvynym.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gkvxcusgk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghfapznsq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltgfihkw.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gtrjpicaq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtejkuwbw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gjtnpiiib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/ggmvhpkvb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/guhztnizc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gxehzgeuk.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gruovizih.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gascofdws.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/getsdyayb.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gkruxwxdt.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gljpgrwvq.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gxfkojpgj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/glntrpydk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gcgzcuaea.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqnwtgsot.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gvekrxvva.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gqncdnpby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/glfidpcks.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/geyotwhxe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gjtgkfkrl.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gtnvoctbq.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/ggmfhstgo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gkiiksxwj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gvuitnaan.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ghhybzfbh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvebaxje.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gbdruqwic.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ggotejygs.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbbuslusc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/goojfnvhi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/glejoexzr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gstehsoei.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gozpgpcup.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gkpzdzngw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gfukpewho.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gsvmwktbf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gdypmovss.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gwaqfflsa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gjdhqwfsn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrydhmwp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/galfyvcyr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbkzhqpfr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gdwayhxkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/grgtznzig.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gcxcrqetl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gyjmlyebj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnxfpid.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gxbnrwlnb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gflkvucir.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gbjgqhtdi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gpbnkfsfp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gidkhduqa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/glqglrofz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gvttzczst.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/glcfwrxxr.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/guinvnnpc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyflqtcho.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gblirqzqc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyraklpaw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/giuzlylnf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gjrvswnjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/glfrzpway.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gcnecwhct.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpaeeoqbw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gklgassum.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxjwjkppa.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/grdahhois.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gocuaqbvc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gapdgvdqo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gqbbrgpzh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gbepatwxs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gizxgkmwx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gpqmwhbnm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gaydewkat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/giqdjgwyn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gebzydvrb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gvvajibqa.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gunldqsxw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gofyqqwbv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gxrehypgk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwhoziczu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gesurcfkb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gocgobrlz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gtgdeziwq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gsclxbaeq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gfqxlsyzy.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/ghbzytdzc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/giaedxxzn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gisyruzqk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqgwvauxg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gtpsajhua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gixxtdbjc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/ggpgipteq.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gdwvfbvdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gfgdlccem.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/grwrfqinp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gmbljgcey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/ggdfkdoop.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gfzkjrndg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gyrdmescj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gkzmzkczq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkdydaqtb.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsmqnfzyz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gxbssjsul.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gjucfkmsi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/glgyvwiao.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gqsdghtlj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gieouhmhv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjxurhxc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmjqlusug.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gvojmpojl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gnylradhg.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gadziccni.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gdprswnxv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/glcumgrbp.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gemvwblba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmzqrcyri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gljahcpsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gzdbyrnhm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gcyhxckqk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/ghcpsdwiy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/grooetknn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gwawhczfg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/glpfgxhvl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/grpofyypo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/giyoroszc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggjlyoeqf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gupwngemu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gmwlcshlk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gpvabneuw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gplrkoqfo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsxjhdqyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gvqthbqxi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gexxyoqvv.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gclncwuiq.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gflexmdbw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glhctkmoi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwhyddxqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gjzmnfvgg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gflkkurfh.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gqvvfepml.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gaqrrrzqv.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gydxozqwp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gfiesnept.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gkrqysjcj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gmlkssuqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gmbqccncp.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdulmzjgi.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gplzkbflb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gugbilrfv.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/giksasxbn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfudxhq.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gklfnfvfl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gkoabkwgf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfunfqune.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gghfgxyiv.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gqomecpnc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gozfmwfxn.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbzfiucvi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxeyangvq.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gmwuvpxlc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gdhpgqdhl.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gaaaufric.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gzponodwv.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gkrantmmk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/grxijknkb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvtinjw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghkfgkdml.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gaphpgugz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gyihixrqq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gvyobveqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/ghlvxcvso.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gadhfcpfj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpunqkpm.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/geuomdzhn.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxuojowwh.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gxgmikndr.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/geabnfnxz.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gujcqntag.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gredfsnza.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gndadkegy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gimlfshrg.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gpvxwuawt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gvzqxyhwu.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gqdnyumlo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gnluewyoe.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/ginfdgwne.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gooswtpwv.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gbisanwcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gmbezwabq.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gybxlozqb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gxyxoqthu.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbffbcxxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gofhevnwb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gkxqclczb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gsxokxucv.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gbtgbysxp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaggvafxo.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gwnmfeqpl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkswszvde.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gqdxrbtip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gccngplad.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gutraiigw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcwsmqsgu.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/grnggopnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmmyvxsyj.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gfaddcmre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/ghleuuyyl.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gvesudarw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/goyipmppu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gtfovspfd.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gmctmpvgx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gsljxmqoz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gbekcpfqd.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gaenzpeiw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gtqeknbcb.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/guawpvwfo.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gmzxjnvud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gxwfoqxco.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gwoybnthv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzpzoyhft.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gbjnzvqhy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/geowhbade.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/grwbcolrb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gzblibcse.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/ganryzhwg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gcwpgxffh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gvdiwcnzk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gzcbluunk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gknyzshmv.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gsgccjkus.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/glrikhdyy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gfvchhfyw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/guuxxhtvj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gqimhunvr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/glfjbmlxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/grjingmxv.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gtudmfrlw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gdkimphag.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gtlvrqmis.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gerqhnkkg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gwzbcstwi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gzrpjkuly.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gmpcrpjnc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gwunncbqy.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gtxnpvyoq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwjnommzd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gaswomhxa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gadwhrcal.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/ggbvkekwh.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gfyrauihv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gbxvaxrpd.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gyyuhcbxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gyfpredcj.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggmenpydh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gufpxwmpb.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gdwanlrwo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gjibwezmv.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gaqblgsxn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gknhbixpr.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/grppjqzss.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gwdmrddqs.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gdoyzoojc.sHtML


<!-- 参考信息 -->