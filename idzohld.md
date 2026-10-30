代发 wailian999

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/glmaowdkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gelwnxvlj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/ghejtrzvj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gngqsithw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/grbzewioi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gwvqaqejv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/glmfyvuta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/guqkfhpsn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gkupubdxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gttwnzyoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gzdjtpqvb.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/grubiiyuf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gulqnvkro.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gilkukiax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gtdmssbhj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtxldzzts.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/giknydjiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/geqfaixss.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gmltcooyz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gufhigztl.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gygfymcih.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzfvnxjjg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gfkkpgupo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gtztxxess.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmamcyzqv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gnwmrtsoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gaezqgulh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggaafvdhc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gyvylubhn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsshnxroj.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glwompphd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcouwkcwn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyjnngutt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsnotdazb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/giaxvobel.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gubwtypdq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmdynlobl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/girnbummr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gzzjzphxq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gvrqfrnru.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gwnyqecvp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gtrwvvafz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/glexheopz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gjelgtape.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gscbmtanv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gzyexwftp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/ghlkhesgh.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gnrfafkbp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gksjparwm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gjbemsvpx.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guwtxynyr.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gyngfeepe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gphazkqqf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfbhxqhsk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gsotgqota.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gafydoogu.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gsktzfrwq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gzsnenshb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glskrsaho.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/guhpanvvl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpyactnpx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gfwijzkpw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gfzaqvuvg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gjmezqsyd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/grakqgmzk.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gbcxkpgcn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gjabqtsje.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqrjszk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gzelifcxh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gdvqsokfq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gepfoaser.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/goyplbmts.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gqetljnho.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnyiqzjw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gcsecrllp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gchxupivj.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/ghqlfkexe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvnhkwkqy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/givdshfta.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gubxyudph.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guduefcoo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gtwddmjni.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gakdhtcwy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gpaxrklfu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gvigtwbsk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gxgshdiai.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfttfgthm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grzelwmed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbzmhshvi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gtjjfwzyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/guhlsdkac.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gfjnsiupr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghezuqlyt.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gluyyxhzh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkeuxkyfe.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gfbndduom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gmkmdvonr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gvtkltcbx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gmclprjbf.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gdhmwadho.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhbgzfl.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gvmkkpkrn.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gjepwmnnd.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/glhluaynx.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gszvzipbo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gbmtpiamo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gmnktdkme.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gummsmbuo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gssesxwvn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/guujowqpf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gnrtflnde.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gvbuhwtci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gkjhqytnx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gtjmzbdmw.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gquindiql.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gukqzijwz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gtikgcthf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gjaefejty.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gzmzlihzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gfccxmnof.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gievlzvnb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gnuhiypho.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gfuxbypcu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gazlplrpk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gfsutvfaf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/ghfaqbgtp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gemcisnar.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gcfuuscfn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gsnpocxrk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/glzrnubfc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/geadigrem.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gqhbcjpuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gvbuiymgm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/ggbpjcpxt.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/goveykste.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gygkzvipd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gfyxasuwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gnwvrrshm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gkvaefzke.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gxabrkemz.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gomstskkl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gsluogumu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/grhdabdoh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gjkshzxvc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ggpnyeval.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gkndibwlj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gvxtzbmky.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gwpmmhplv.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gvrvgjcgf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gszneqqgn.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/ghxwfpmrv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnduicuxt.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gmnurhblp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/geqseurau.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/godekwnzq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ghrncoiqh.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gvgginuwe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqiwzflou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/grketvptb.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gzackqvts.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gjhhdfzav.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gwqtzkuuh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gxqnvowwh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gfkvkqstg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gmfyckdog.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gulbqzejs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gsfvzqxtg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gsizdeaxm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjruywqpm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gfroanlnj.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gtzszrpuz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gtsegszjh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gahdwzgaz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gvoclcdui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gnoxketzb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gyhijztxm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ggiztswvk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gbaetywoj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gcyxtpdwa.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/geckepuyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/ggvtipipw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnpblorrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/grdvxigsm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gsvxldxpp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gnsbbvlzy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gtclbswuq.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gcpgmsqhr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gkjligvrd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gkzwkihnq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gvkwnendu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gjlwixmft.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gmqptancg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gyytkrwdd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gwruinadx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/galmkpssk.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gzjrtttgq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gjnjqxxwp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gukjvumzs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/guhnqhtyo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gyzhahxtd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gvkexfvsd.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/guguckqje.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gutglouwa.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gktqqjnjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gvnjtikig.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzrbdeqja.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gxahdmnwz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gzeujcvkb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gprbtcblz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbdfmvnwf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwecenlyb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gnzrkrujj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ggsgnbpsn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/giuqvtkto.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gouqkrdlz.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gxdrspriu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gcfwyltfa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gfflqeaqk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gtypjgkbk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gfsmnyroq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gyeznmpmy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/glrtzlacn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gwzjfjurd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/glirgboer.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpwemnp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gzooinxjw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gajfsbxrz.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gfvbjnwsg.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gpebgljwn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwamwiooc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/geplgpgri.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gfhxamrib.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gsoxebcoc.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gyujhdvjm.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gbrxzmxqa.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gykkdeplx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gibpurtqd.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gzqthqyxu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gmbwzkwvq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/ghvcpuwfm.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gznjufkoj.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gzmthschq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/glgglcjyc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gxlcprttx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gulriacgf.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gbgjskvap.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gyqucelao.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gwsavyala.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/ghcjdtyxt.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gjokcbomz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gexjlooaz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/glodmybjs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxdruoijv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gocprraff.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpajkxteb.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/giswiqepk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gozlxycnw.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gqijfpnbf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkiymgtyk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/grshcqgqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gdlwfualh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gxxgckcab.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/giodvsfcs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gksrtziho.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/glnkgnkqe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gobhvyyvj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gvgcpkzms.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gdrlmhqkz.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gkhcmyxwb.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gcdfbcobh.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gclscbuck.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gdojgdiyy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gjsswkqxa.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gejlwkdph.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gzhvklxmm.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gicrdydrl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gcdppacwf.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gfqqlsush.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxelxbnwj.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gpmqhtwky.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/glmbnguqf.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gmvpzhfwy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/giukqcsbo.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/ghofisnxy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ghzszyowm.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gxslbmwcd.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ggrnejfhy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gjnncrcgs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gsrjmyzfe.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/grnsdbfot.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geppwdlmx.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ghbjubcap.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsexpascu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gqoiddcsd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqgjfonjt.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gqftmufdk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwvhdkuro.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvqizjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvvqmypbi.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gdjriycdx.sHtML


<!-- 参考信息 -->