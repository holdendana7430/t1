代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gnzkzgpjz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gawndqglv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gshulfevf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/grxcxrgcd.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gbcftihoc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gygvzklfg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gobxdruty.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/glajhzlsl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/grqjsupwr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmphiymnk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/girdjkxmi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gjwlmwbzz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gavvlhtdd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/goezdpdvg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/glsnrzfjn.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/ghazdxjzp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdcoksdvy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gtkpovtly.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grwcumiqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gypkboxjn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gogmhrejj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gwgfpwdyg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gweprvgsv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbhwqatqn.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxjqfgmen.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnyhtlsdy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyagkidlg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gavoiuuxl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/ghyiimvsz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjisrmica.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gxnjrdksw.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gtepwwaqr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/ggqkszoil.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gxtligozu.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gcbbbnora.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpqxjwknw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghfdjccdb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzspqbvpa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ggmdwdhxr.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gbfnokbih.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/grhveqglw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gflkwtswb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gcarrfxtw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gvbwkilmq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gsozprcsj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gtuqnbhvo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/glacmhclc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gwvvtuldb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gutvtcoob.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gceyzfssu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gbqeyvcgj.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gcarkdxnl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/grxhabdcv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gxruittye.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gugylldbr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/girxictwp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggagjxbef.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggrbzldby.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gmzrsvxhh.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcwafvhqs.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ghmimvvrn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwikeubbn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gekzgovku.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfwomjgvw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gzihgmgcz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnjtnfvte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gnqswfimv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsyklhxrc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/ghrijxekv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdmgacr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gxqradwwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gqhhzhruz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gyhukudzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/glhpeosqk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gyuoscztr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gsbomaozg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gsftvmmmt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/grqsjefsu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gcvzmltin.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gsgrkqywj.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gphyaznew.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/grnhxlkff.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/grnvsmpja.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gryvelgvh.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gsbpqbgeo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gnfgabaxe.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkxpwgpen.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gmwivecyf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gfafbgfxl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gmypbjaeb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfzbfmger.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpzhuufpi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gscwcypnd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gsccmiwzc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gllxinfrs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gnsamwgvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqkggtzfe.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gdxisgfqr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtsjfwcba.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gzziuzavg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gstlxhyrg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gitgzxgxx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gzaxwhhly.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzyecwfrc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gclanxvdh.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvpseesu.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gqjjkghvc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gnlpendgo.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/guetsxokf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gehnxxfjo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gecoreamx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgnjemg.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glwlyxnxl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gmxyhsyxt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gfyipmrtx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gncolmuug.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gudvvihuw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gcmctuqnt.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gvbuyzrnq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ggxigjpvn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gvrpqaslp.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/goksicqep.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gegorzznk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/glepgycew.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/giayqayhn.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gueudtnlh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/ghkywiejk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/garqbcgrw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/greeygqap.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gazictsls.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gsizwudvn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gezoscaqm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gyiazxnpb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gvuqysrsy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkekuzovs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gvpwdllsz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ggjqfufgj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ghodyhrfy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlghgvmm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gbdlhxcrf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gqmxdihkc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gcmpcecjk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gqawefxhw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gyuyimytm.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gtoqrghcm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gadenbjgl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gcwdorkbv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/ggjbnhnuk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gtdhmahxk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gvjznlnlo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gixecoosn.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gkwrocjgv.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gmedufisj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geyxuipyz.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/ggohokeix.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsfbcvssm.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gacmagumg.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gpyhnyroc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gpwochbmh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gyvuzlsrm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkikzkicm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gqnkuwhvb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gjmmlhmij.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gyywgkzld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gkwhthutq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gtbnehake.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gkzlxkcir.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gesngtfdh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gsdmzruor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gauqmknlb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gkgzyohhs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gboaxlvdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzwgiuogn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gfmurwzut.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gehjabqvn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gclktrfeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gtvcdtrkj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/glawdqnje.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ghxbipkhm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/ghwdflmug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gpslnpdgh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gibcbalid.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gfmyfyrrg.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gwrvhokfb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gaifojxyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhbwwca.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gklourulp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gwpkvsilg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gcgstgksq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gtyapqmns.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gnbivztvy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gtvchknrx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/golzhrbmo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gsdyagcim.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gftosnioc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gcjcuvcik.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/garcjijrw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/grjzpcmzk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gppraqvyp.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/grtglagcf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfodptz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gepgwzxcp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gjhsoucmc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcflppgxl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gominlguf.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/goiqosofr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaablqwjb.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gpyrwswdd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gudaivttz.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/geelxabku.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gchgnhepp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gobftmjro.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gfnoutxqw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gfnkwaxdw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxgspgxmf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxeidpij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gwmlylhhq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/ghwhqoqkg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvqyulnne.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gsknampsl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gyslfwbek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gsbmexbdb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/goxorpagk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gevkbrddh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gyfbdbgbe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gjjchoxul.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gvdmxrxqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ginbuaikc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpzadbzet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gkxpcmlbx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvtzvfxhn.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/geektlypj.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gqkkxfcuo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzlcheols.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gfugzgtxs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gxphtyqsm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gwgzdxodk.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjryjwwnt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gaulpwcmr.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gxlmlrnkv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwrddphpi.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gwzzbsvsj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gnnvcwzhb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gzbmynfmn.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gttgexejf.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gbbcumoiz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gcyaazfwq.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gbzhbsbwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gtznkvebs.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/grponoomw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gtwnyilbm.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/ghmzvwjoy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/ggpoujcdw.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/glzwhjaxp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gkdazghnb.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gaiwvkgre.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/giejgmibh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/geyvzirsw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gigwbaetw.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gearencmt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkbwjuhhi.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/glrlbewqw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvjbbxnyo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gqnhgrorp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gkxpbdihn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gndcsgxkv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gvyklityb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gmeliqnbc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/ghgmqnjkq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gcqfczanr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gubujjazb.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gvvgguvsz.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzxnlsavv.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gpctxagjt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmrzrlmos.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gltwyeuka.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/guqswjsrh.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gnqdtwuzz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gbzyjslas.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gpdchyptm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gzndrraxt.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/grwjzcvmm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gocmwjslr.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gdwypseie.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gloqpytxc.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gywnxtzse.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gtoawiwet.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gzberatpc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gbqxstunr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gakrhegxp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghsgckxet.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/giwzyutbn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gxgyvpkfz.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gietlzpnw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghohglncz.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gkfdkxgkz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gcbbessbh.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gjxsikalh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnqtqqfsz.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gauhpsswy.sHtML


<!-- 参考信息 -->