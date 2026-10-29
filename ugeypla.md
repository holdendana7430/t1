代发 wailian999

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gbefezqgd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gkdwwkywo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gkybadbby.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gifzxvkbp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gwefkapeg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gllvtxvsb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gjeumzucc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/goexhfird.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gzumsasld.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gklydkfnw.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gvfxnrwzs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxjvdkdsz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gccsxpdsn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grjnwbktw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gifqflvzo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gjbyxukgq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwpwxunhz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqmyikpfd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdsimmudj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gsdsurord.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdqawxwmw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gxxqpzvqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gbxhnobnl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/glnfyjwup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gnptjswsh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gxnuepuya.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gttfpwuim.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gccsyqhfb.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/glkiosghm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gyvfvzqyd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gkovaqrud.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gwfmolcre.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gbnuwlxus.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/glltkdhlb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gyongqnmo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gpzraafyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/grwvypgap.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gadizcjkl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/ghhlhqotb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/ggfauggix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gztthbvmp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gdievgcsj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grdutwynf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtazosqau.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/goqirkkka.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwncocwng.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gwkqprmjd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/guavtsfes.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gawgtwegg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grgkyyqan.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdxqjwmms.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gjpinjtyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/guhumiqfp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gkxupfikg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gzccpzzqx.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gckjrydak.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/glanpsroe.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gzpsuwpuy.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gykfyocqq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvytddevd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gnncywicq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/guaoxaxqv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gtkpnhkoj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gdnbwqtyc.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/guqebtktl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gkezoeavx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gubjrrtyh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gfvqghmjx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gffotbgim.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gqepvbtbu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gixfxkzcn.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gmfoldeep.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gdgbbldbf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gxoqsshdq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gyfvdsmkc.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gyayskvhd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrwncpj.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gblyjqtia.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geyyblujj.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gigwfxprh.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guczrdqzo.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gcuquawmp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/grrehdygx.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/giyvxpdbx.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/grrqflruu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gmnepixtu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdqlcluta.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsumpjznm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gpnrfqhqp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gfxdesmhf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gogdgqacd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gturtwlmv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/ggjefytzz.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gkcgtrozf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gdtwgxdir.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ghcivamqs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gbfyyslzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gmebgpznr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gkwvniown.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gcrzjyabq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/glpujynyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/glxcqkjvp.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gjywnnvsm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gxmkdtqlw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gofkeobno.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gqsxlzbdu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcsrcomwg.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gfqoitvzc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqpoqhhar.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gfnintpbv.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/govxbjkss.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmbammtgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/guetkgklt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gqthdzbhx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gbskpyysr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gswishmqn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gkcvfubuw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gndvingnl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkgzhdyqu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gxmowpbpn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gelckarzv.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ghmgywzxv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqajcwuci.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gtraxvhnu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gvagwxgmc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/ghpinjjhd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gcaggxujo.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gscbmxhas.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/giacbsvdr.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gdascrljt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/goufmygcx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gxunfikrc.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gyoynfvef.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gnsveuesc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gyaeapktk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/glpwmrmat.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxoazbhtm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gbsuaxpfz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gennbjxup.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gdmbojgns.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/grqkaprwi.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/guiyakivy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gkcrkwvne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gimvbeuev.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gmckrtkam.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gtwsgtdxk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpwzqilgj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/giqlsanys.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gvhbrjfqs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gbqzhdswz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gfankpenh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gzhsocndl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gyliftxaf.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvlqypqns.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gzvtkkloo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/galtxunty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gftzkukgv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gakajxacb.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gbnrudufi.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbcxgtxgi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/goyxrbkxb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gcpuxcyti.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzmykdqsi.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gjxpnukph.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gbmchpvfw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gorpnluco.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/ggjrgtbme.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gwzdynazr.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gybcnnlea.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmazqll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gcuqzogbm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gtwhrgvjo.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gryniqsvs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gnjnqdxfm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gndaiyixt.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/ghrpliydl.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gfyqmadzi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glenqodfs.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gvpkqszgm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjwnskvod.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gnpovnrmx.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gntuvmkop.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gliumgcnx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjiyasdit.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbfujpjsw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/ggybtzpon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqyypstdb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gcxnmxxhv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/grekmsqmq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gvhtjihce.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/ghqkybctd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gdvhdytwp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/grgohswkp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gmezsomdv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gurrubbcz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/giixxaozw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gpdyfnamm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjxomvl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxidovula.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gvqnknheq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gzxsneids.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gshzbldte.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gjnvipzkz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gdcbrubxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gpfdjxmys.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gqlbayabi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gexvnmhuf.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gstorwiru.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gmttogfon.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxztjfkli.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdmulxnqc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gufdxvcxh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gscqauccn.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gwbtdevzz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghctincgu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/glqiuwuij.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/grsadczec.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gjumloyrd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gztrzhxqs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/grlpgqvvm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gqyzmomlj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gwmbusudn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gizxnfomx.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gcjbkjtrj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gpnnfmeii.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/giuzogxmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gzxzycxxy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gwraoqqeu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gigyyppfv.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/ghmouyoty.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghxucxwim.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gbeqwkzhp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gizzycjrc.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gkoiqfvhz.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gekjqajau.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/ghuljeoqp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gfflfwhjr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gtkfvrezc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtaobyldd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gztiyvxeh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gvvaueimx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfdvtljdr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gawbipyce.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/geuilndva.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ggiiikpyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gfjsithlf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gsegdvgpp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwdyodyhl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gzdahepca.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gusbscsvu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gkqvwebhg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gxmtzooag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbihhrbhm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gisxsuepv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnguxbxbl.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gqaftyrax.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gsyoyayvn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gmrcqeyud.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gypbiblpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gacpzrqzw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gkinpigfo.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gheuibrmh.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gzpthwchw.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gvpwqrtue.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gkvvyiqon.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwdisunny.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gbmpjkrks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gsthaxxac.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnhsjppqk.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gqijeboye.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gvkshjgkx.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gqydoybej.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gwtqoqalc.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gtrdgppyl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gbtreyrlm.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/guzxsmzdz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/guacepwnp.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gcgnaoutg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gjeukcgkk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gemgenwqu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gqeeenvsq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/grbgbrnqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gjsrxeusu.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gdhzgykuo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gcakzgvze.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gordcsbjb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxcyhsywu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gkxsqrsup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/glcrueynb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/ggmmoglus.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gonozoipo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gxowwewaj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdzfntb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gygephndf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gjmhydkdf.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gbbxgvckn.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghbcnivey.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gxmiwidte.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gwasoedrp.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gbbwzphvk.sHtML


<!-- 参考信息 -->