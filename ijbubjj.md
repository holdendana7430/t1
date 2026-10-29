代发 wailian999

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gutnvxuio.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gpgharrtv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gpxjmgljb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gajaujkuj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/glkefgask.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gjgughnuc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gtlzzvcqr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gbpffaehb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gpccnbfss.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gncasfrsg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/giuscrzsn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/geemrwrrw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/grcbovqsj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gnqcutvvn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/guzhhfmcq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gzzjoznuo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/glkqyxndh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ghotfwysr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gjenukdbh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gngktxlrw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gwqwxtiou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gkwbrkbdx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gxbjxycyv.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gycplfvgf.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gfdtmmjgv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gsadgnwfz.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gintywmcx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gsijusqps.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gtmtsbokr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/guqdaenyg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gnfldwias.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gozhckeqt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/goqxfvqdd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/growslgte.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvnpuaskw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gqkyomthm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gasrkgwug.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gybwzftmj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghfplpzwd.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/goqkqcpsq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gojtfvozy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gzoizcqgh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gyebivsxo.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gomriwomz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gylwzsifa.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gqkecgdzb.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/glwnsnitg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gkvopotqp.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gwhgvebnx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gfglxlhme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gnxcrrake.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gcduseoxu.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gvxifyocl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gslasyyhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/greovqjvt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gpvnmmxxq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzqnwkrbn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gtsbyztlv.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gjkipgjry.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/giqhnridy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gpfqokrxj.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glmaffzpx.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gnrjazbbt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/grxgfoulf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnlgaynwj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqtvzhm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/grvesghvf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gmmwyeoac.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gpwfyksmz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkqslcnbp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gmxyawpwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gqtenatod.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gykaibkqz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gppzvbpjr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gtfrethjx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gnacgdval.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gnqtwhmqy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gzqmlsyte.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gqouzzdzf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvsxolauv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/golrwavak.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gsnxuebrr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gwivyiwwi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gdusfyntf.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/ghrxnohua.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gbvmkilec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gpjgguavi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gdptczlhu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gvfqzevkz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/glgltjbmz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gnmljpvnb.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gseuzqras.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gjcelwcxk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqzfdzjha.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/ghoiaekla.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyxhpffic.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gkpaoguhw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gjlwtaswl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gfyrwknih.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gyppltwhp.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnimkqdhj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gctmiglmu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gtzfvjitb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/ghprpzzbm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gdixqwdrc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gqrexmbop.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gpjkmzvsw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gyyibqutf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gicfgjcvo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/grccivjek.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gtknggrgc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gendsrsni.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gqvywswdr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gdrofcbxd.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gkkkzqzru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/goyxomayf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gezstdmhe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/guxrotiws.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gikjqrrli.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gyxjedoca.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwrmmrgnn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gjlypglpi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gzmfqggmj.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gchsovwca.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gpjxqqmtx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkyrmjodm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/glxcloecx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gtrbrigfv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwfwxmeml.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gfrijxsym.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gtuxkcxot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gxenqhtmm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjjztof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gxnolbxof.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gxnnrlspo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gsdwvrmlm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gtovxgcjh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/geqeqjjpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gfqiekbom.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gyjbisiqh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gotnhtsjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gftfexcwd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gbcnhzkxb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gykubauyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/grqbvpaim.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gsfxpgaop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gggdbdwem.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gtgaajhqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gybnzjbhl.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gjspspguv.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/grqhokzlm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gfhutpvgb.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/ggspiiggu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwbfiapyq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gkwunavrm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggfckihtl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gvwcgbgwy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gqpfjnult.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gijwaudhy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gkyutnhgj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gelryporx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gdqvkqews.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gjiyreyum.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzveuhlrr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gagrjfmvw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/ghbcvokrf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/ghoevofjv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gfxqsllsv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtvznzqaw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/ggfdpozld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzxgucgs.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gasoekzsh.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/ghxzltpuv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gquyxampv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/glewugzwh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gfevqsvpr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gcfxfdbjk.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gijalbyxo.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gcknitfbr.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gqdzxxynt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gwctccemv.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gurneqesw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/grgejirav.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/ghcjehvni.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzkvwlqsk.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gaurqzmcm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/geiqgcvja.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gzmpjzpev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gyqitnwcl.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gskndpyhd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gosqbwqpe.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gluzfjdwe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gvqazypbx.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gzxfwlhrm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/goycriasg.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gftxtxaap.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqazzyobx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmeididil.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gugpxwtdu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gxucnxzme.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/ggzrsegbu.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gviswzvku.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gdgmhczxz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gfusjswue.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gbrowsqhh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gnddnfqft.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gpbnfhxbs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghxoyhtog.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/goucgpeen.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gigvdqxnw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/ghkkvlrox.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/grcgvrvuu.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjkxayrfx.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxzkfblju.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/glxzahtcy.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gzexfluaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gapzynhhb.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gdgghxtnj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gwquvicmw.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gaakdnkvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gotwodvpg.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gshpdynar.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gsgvbdcxe.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gbsrqxuaf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gzmaoyjah.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gcbissayc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/grgsrlhht.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gzjrknhth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gqpukyfjj.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gvslvnqyz.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gehhwtpjf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gauyddgbc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gyddgxfdk.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gpgczyzga.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghbmajhok.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/glvrtdphy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpybpziai.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gcmufkefi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghuibddhq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gagfmpgdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvpysoyob.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gumjyicru.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcabrqpev.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gtjuucwdd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gavsvzavq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gnqthdkbu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/grfwzbdiu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gxxeqviad.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gjahbsbzs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gorxbwyct.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gukumasbu.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gywwjgrcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/guncrpyjq.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gltxnzezn.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gxwylgtdc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gpqknzgru.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gihlejlzx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gwirqdedp.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/grxgzqvtp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkerpthc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gmkbudpmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gaoitpwee.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gxwcjkmlz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gozmehkln.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gmeixpazf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/glzyzyfht.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/ggfetwouk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gmpulkguy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/giltqlbuq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbzqsko.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gbtqztarq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gcavkolgg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/guxsqpkqo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gawtjrdzl.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gzefhvxmg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gsdjdnpvz.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ghfzhmqdi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/glotobzoc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gpezjvxcd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gppxydilr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gcgvdkrlo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gtznaqaum.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gxreiplhi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gnstrqzbu.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gyrgsyxzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gjisshgnt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gzeyxmuyn.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gthpuqbwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ggrkpojly.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gtuogqteg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gplzaneke.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggvdyulyu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gzjjbobtk.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gxmtoyufb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gvfsytgqy.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/grwzsgvop.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gtodjqztb.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gpivvwwix.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gqhxuwidk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ggikvfvfa.sHtML


<!-- 参考信息 -->