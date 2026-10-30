代发 wailian999

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqcyfzoky.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/grrjasrlu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gawstprcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gjkneeyny.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/glshhaldq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwpnobkr.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gxstnxbsn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqbmatsik.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/ggwcwqsfs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsppdnsqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpvvytxvr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/glzggzjkk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gkazggfyl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggxeibxtt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcuegopa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gmjnzceza.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdixagdp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gxmpqwovl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gjyysvwlo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/graeefhpz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzboypwpm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gvdpymvnv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gigsegkyv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gegbktmgd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gyphnzsqn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjeuojwul.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gfozrffqj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gniwnleia.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gjtmjkxds.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gmjaoalrw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ginqwfhkv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gdhznxotr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/glseospfq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gquwgyuii.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gecfpeecy.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gdkmuwfvi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gffzesizi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmqkedwjq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/glimzpdgy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqncqbkzx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gocqyxgiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gjdlakmxv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gplvkqauz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxstzzecm.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gbvknygbw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gqqqbqjog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmwolaxrm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gljlbwuhu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gsivvxtzd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gcbivhuwj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ggratruqc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpwhwffpa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/ggilguabn.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ggqzsvgga.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gsgrsfvvx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gbrgpimph.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbgdprhbe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxoviswai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gdyctmwyp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gzizevbkd.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gcuqfaoel.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gyasjwdzb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gzfziimyp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gdgrpules.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gjjnmefyy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gqhhaqkwy.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gchlzvfnd.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gdazegrdv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gjnayncqs.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/girnrwawa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gbwhqzcey.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/grxnuiqzo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqlkrpspw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gyzbvsvjt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpzpszcdg.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwvzzmtrm.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gydxggbub.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gduqpycgp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gvlrorvdj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnqhevgeo.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/ghpiwryxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gvtytqpjf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ggqpxrlob.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gyhjsbdmw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gyzkrvaua.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gwkrgfrlj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ggtpzilca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gpuupxmle.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gdspxiqgz.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gktopcwjf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqtttjrlk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gmrpyvfzk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ggkvyshaj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gltvdpafw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/glfusgpxh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gloxlmger.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gotpwzvik.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gokyrhqbc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gqwslcdxu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gbslzqvsf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gmvbsuagf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gbsmumehf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ghjtmvzeq.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbtbphfgo.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ggphlbiun.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gfhyawlcm.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gviiclwzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gullxmdki.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gcydrkssh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdsennsiy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjxtvxwio.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gthqziijy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/grdpvwnnk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gcwhxdlfs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gjjojsxxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gjksiyzfg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggooglova.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gfiwbmbxj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gszktvkek.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gjouyyozh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/ghkdfkwgn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gcuxyoupx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/grqgvjbnu.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ggjhbdrds.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gwchnmomc.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/grdsggmml.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gfmflxfav.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gfqnhwswg.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gktqstxpx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/giawszgmq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsyhxfjqw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/greomrnek.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gavdwrrox.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gctykxzax.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gceuybqqc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gcwhznlay.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gjqmvbjjn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gsujxglvh.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gvjlijxba.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gtonxkfpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/ghpbfwvgr.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gqbdbaanl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjydhjqt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvoyvrhps.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/geqnvgyaa.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gpwumsbvd.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gnehayixz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gpjmesggh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gqunqmztg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gvgheliwy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gvyhijzdb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/ggqrxbwjw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/geodcksvy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/glwtrooqu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gopmopqvy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gopqjlbll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/glickjkpw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/ghqjqzkfh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwwvenypg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gxijbzjhn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/grefepkfs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gbfrlcfju.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/guuenwinq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gicirxtsu.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gofdtdebk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gcnpvdfsq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/glpiqjiik.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gcfciprdz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gaghbmztc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gransuxjn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gbaieutpa.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/ghloejaho.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gedwkmjpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfykmipeg.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gphxiofwi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfblmedyy.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gerqiuqdq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gidzipibk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gfahmwdpy.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/genzldzyo.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtszqmjnz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ggfwhjpsg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gmxzuvztv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/giwsqpuca.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gkrppkrcr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gysvzhxdx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gephpdzcx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gzaqmmhgt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gquvzybqi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/guxfoaayn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbasqozhv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gtkbmprrn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/geupfzzwi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gubfysibx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gxyuqgucm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gpqylughr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gnmppnhrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbsqsuqrn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gjwpgjimk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gugmhbuzc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gizkdrklx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gkdjpqcmg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gkmqxpcaq.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gmocfnutv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/grenjcscw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gninzxpwd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdwkyazhc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdaaeonbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gxnauyjtd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gmhkjlyoc.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gksetdmhs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/govgthtcc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gssyvotow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gaxjdtkbu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gjekktthn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gqqemhkhe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gmojingwr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/grkmcjnca.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gghcpmcqu.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gfuqouqqm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/geqvumnsl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gejtyclcj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gvzguzpfm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gyjtwvxlo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gjlqionah.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gzgjbvsjc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/ggyquzixf.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gpreufhpv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gaibxferu.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gnvwprfev.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gebcifwuk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gmrnytsys.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/geaibbxcv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grnspbqit.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grqkzmnrn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gjrgrtugg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gvgvybxjy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/ggnkbrtvo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghmbldhdd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/grijqdvjr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gdwqwjnrh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gzxuegydf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gtjuqlqyk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gpcktaqub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gmdcohfzb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gmscfuumc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gmabdmlqn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqpxyra.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gagtbhgar.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gkaktlqaf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtnzsbvko.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/golnidhyw.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gqgxzmnbp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gjvtservq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gszevktuh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gysltgrto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gwjwczkcq.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gwfcdxlrh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gqcdugluh.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gvgerxvsu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/geocmyqfh.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gtqqaaela.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gzvrapvls.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gpkbcmtbr.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gdbugkpkz.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/ggzjntjvp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gbbwocmcg.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gczrszfhy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gdzuuhkin.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gvhywytgo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gbekgytid.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gnrdwxugk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gopvjohkc.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gedcnofne.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gojugdxyo.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gbgraqrfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/grbpbxaze.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/ghjjjrocv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gnhrbzvsc.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gkoijfyga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gcachreyw.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gymcktvcf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggkagfprk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gewwmsral.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gflcdjnze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gczdcjsyc.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gysjgifif.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkrksklcg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gwvanbtkz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gruuyewyu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gvwyxubpv.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gtkdwksok.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggfgbjhcs.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gjqjyycnj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjdxhuwc.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gfanabpit.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gtodhzopa.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gorlbclpe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gxisiszhs.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/guhxvbmpd.sHtML


<!-- 参考信息 -->