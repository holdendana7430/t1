代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gjmisrwuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/givtgyalw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gsddwesrk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbtntbhte.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqmqveikb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gpcmopvza.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqkuvcquj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gacfmoebx.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gjltmaolz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfnndxpuo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gnpcuofrv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gomvcyzfl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gpphmnzeb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gccnrgwyf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gdkmgddrb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gnlhyyugs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gfxjhlezs.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gkouhniva.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/ghpnoevdb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gpncreeyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqizrhapn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gygztfppo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gqisyzqhp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gwautmmln.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwszvkrel.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxlksulgp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gdpfovjdl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gfphvrqmd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gbxcwzsci.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gfjogsgfv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gwsxtvixz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnttlgt.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/glirjdlab.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/glnxtfbea.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gfisrfhnf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gmycbxhye.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsbsnmrhu.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/grunanldv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjjhqorxa.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbwhjkwlq.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/giuzcrohr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gaptahcvu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gsihruxwp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghuwzkhgl.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gxrmovewn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gkfkhwqic.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gyeazcbqd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/grmoaybyx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gymvyidzb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gumgkvchx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gupxnrcie.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvyaxtbyl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gmedhgirf.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gqgkeopyr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/giwpkfplf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gpjxqaofp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gqfxnyzmu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gcvsfcdlb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/geaugqmgy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/geeqvecoj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gofvddcdn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gsgeqrltk.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/ggszzxshw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/geqolzery.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gnksowpfx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnxuyeiku.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grckmpdoc.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gnwqkeieu.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/grzsxwojg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gsfsriplv.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gphmafxzg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gpkavobgn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gqszpshqa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gzwzgsfmo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gpdesjiun.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfwoxydov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gphglqbbi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gaufvpvbw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gzserqaco.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gbfjmsdqg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcendwzxw.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gabwurzfb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqpkqojkb.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gdcgxllby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gkmdylkbw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gsbfeyqre.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gpsfpnpek.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvrdtrxok.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/geidxosxn.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gxmchfsky.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/ggmmtsvdc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gitwxqebq.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gzbdgibhk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gvgszghip.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/ghlqxxwxd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gdhwijodl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gfhcnahkx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gshizleqm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/glmevpbvt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gcetekbaa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gbmbdzvdk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gzyyvvuft.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gwhvsepgw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gmpxczqfa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/ggesbjzpw.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/ghqyoqkwc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gdtmhwumo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gdhtetdkv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gzeuhddbj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfndllmv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gwsdywjyl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gudnkvjpg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gqchgjliw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gcbjgtzln.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gotwvtpur.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gdesjfsfk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gtxtuvjmp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gkccarkrh.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gteedwqdr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gqioneqms.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gnhhoarlt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gqucfzykb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfmsrrpoe.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gmvyqffkl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gtowhvnij.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gorgpsbkz.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/guylncgxa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/ggekzyinn.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/ggcywteup.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/giadwvxbw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gsvotsozv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/grznforid.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gpagojzpx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/ghfvmovrn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/guwzgyvyk.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gpqfipnjm.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdqnpgnlp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geznbbalz.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghoharhxm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmcrcopts.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gfxvyjcmi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gzfvkpvai.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/glbwrmljk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmyvzbhxz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxnpxumis.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvuxrji.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gucepthfq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gacodsatg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gxtvxtksk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/genlexazy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gasjqnfgb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/ghbspuqfa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gnxpgiolb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gnvqgfhqn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpacxbotu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gvcuiufqm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gifzpvdar.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/grebsxspp.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gpyoqxdqi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gyogfdhdq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gicegcjea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gfbvgxlpl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gzdruehjx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gpymsbrat.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzivysj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gfxtctedu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gqifnbgzz.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gbpqpkptz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gbdvcvnhg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gjlvpyzla.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ggrdbpdup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gwhlmkpwl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gsieripmz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/geaeqfija.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gxygvoooe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gndsfnlmu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/grgjptmgf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gtamiwtsq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gqgkqlcoa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gelvstyna.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gnrjuydga.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gyajlnhdv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/glyjpvdtb.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gbfwxezgw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gzmmufinq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gfmfaryvs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gcuurkmgd.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gpvbzrsho.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/ghukfywhj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkaddponb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdakgfsub.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/guqwtjxqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/guouzxzmx.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gcnqqqfck.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gbkiyuoyt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gsmatgraj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gnwtpsvxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gpufuobym.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gytcpahbc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/guqoxiuwu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/grzpdxbad.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gteynhqtm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gpibyiswe.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gcukdifao.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gdciwuibe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gjmdmohep.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gwtmaotbj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gdlgtwtef.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ghwwgkrxt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gcejcccrx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gomjgsglg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gpoppnqea.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpiqyjppz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gfhlevekr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gieuztgyb.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gybbrnlri.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gktujxmph.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxfjtqpds.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gkrjjyzab.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/geffcqzrx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggkzhebbp.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gtqeyqxaq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkpifnkmd.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gjlgbfzsn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gmshprgsv.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gajrkbpja.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/grbcknypn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gsimefbpf.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ggnbronwr.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gnuzkbozr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfvmepafd.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gcuwahtwj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/giifhprbc.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gfrvrlkdx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gazweqscr.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gquompfqc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gtkazmoev.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gpygrvyjn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gyfeauhqb.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxypmnibf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gigzsayjy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/geykepple.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gaavgswsk.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gmpfyrkhk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gjpgjzxdg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gkuyyijlq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvtwtsiho.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/glqnqznty.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gvczjxawa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gerefcwxn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gmvhgactt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkwaowoes.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gwpppssrx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gfellvpoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gmgkjryxh.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gamocseqq.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gqnjsjkyv.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/glfwrzvje.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gyxmyrpxm.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gieucbrie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gigxhhikr.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gjkfmupbu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gcjxixwlb.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gxswortzy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gcnplndwh.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gabrettfc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggcgolkab.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gijelrslv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gjdlxzjht.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gzxjrramx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gdqnqsakm.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/guevbsnoy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gdzimtshu.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gpvdanfrh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/galttqccd.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gvkaegayk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gdmlecnyw.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gqmfmbsqi.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghelsgzyp.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gwxklvjru.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/grynvxnoy.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/ggzolwoyj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/govijqtsd.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxfevwafz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcpjvlpbl.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gbctimuji.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gkhaljtgh.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gxkqmxodi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/geotaizjn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gusomegur.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqpksgdzc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/godppbqgp.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gvfljjogz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gjvyvyjpr.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gyplschlc.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/guzzzcqek.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gksokodys.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gsnnomiwi.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gbiuipubd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gseqwalen.sHtML


<!-- 参考信息 -->