代发 wailian999

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gbhigmklk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/ggfmbnuer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gukkonmjp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gzlidzypz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gqncdqpsa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gwbcqydqm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gkdwkeuzk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/glgvnofag.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gkqepbiuc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwtesycoj.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gjoppkbrs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjjzsftnh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gdlchjdyy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdvumjtiq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gkpdwxxhi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gycymxddr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gxhvquufy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gptsedjqx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkbejabcv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gwpfonrbu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggacnaack.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gatshktvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gnwpjypnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/glpajrukp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdlyvaxvz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghoacirim.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtujrfnhd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gdzzgzyzw.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/grocxrnvi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/goblignvu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gwiwxojhq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gbewvwaxj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gbhgszypn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gkbkskraa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gmzuaajrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gzlvpmsrn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/giakmehke.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/grbzxvsjx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gnpvraudw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkbaqab.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gkljkvxmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gupbaqeqe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/guhizcepj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghewxxhlu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gnlrjmlue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gsejczisk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ggxxeukxx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpvbcvtyu.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gkjhzyawg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghwwiersh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgsuydqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ggqxgmcak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gyemvxdvn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/glrdjnkew.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gzkvliqyq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/glkgzhndx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gynjeaome.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gnmcfrkbl.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/grlsqizrw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbgyowznp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdoaneyxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmdlkgozn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqjfmew.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gmqqmwqsi.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gpmpqdtcv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gipijojbq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gazsctgqf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gigzoenje.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/glqvyhync.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gfdspjdyn.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gqvnzsqdh.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gnrnbkahs.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/giyeupjtk.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gvakvhrxh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/geaqaiqbm.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gljyegfql.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gkftdagle.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqkixol.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggeyfujaj.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtgqqbhgw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyvvquljn.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcvxeyyma.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gnhkslwyx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbwyksqgb.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqvzmccyi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gfuqtsbsa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gvytijlcw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcezyhgbl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/grrhynpnc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gptqwrcbo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gosaelobd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gnwmmubgg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gjwrrmoob.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gynyyiehp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gbzsqyntu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/griyoxdxi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gdevozrjc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/guduejlhb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ggxabkrlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gttmvbnpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gqtbtyiqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/goxjgpaxh.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gohpfresw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gsdeuzlqi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gqaxjgszq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gffetinnz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/genlsuwzn.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gdgakohkl.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gvostjzuo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/guqlwltbn.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gjejozihf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/geamuqmkt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gxtjguhoc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gewkckxda.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gqitagnlb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/guklqebyy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmixonjvr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gvpcbjjsj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gpwqnjvze.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gdxamdzau.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcaqgqzlh.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gjmaxajng.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbzaucsb.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gfhqqgokk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gauslewag.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gpwxmgvgi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gtxfvntqo.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gakdilpfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gfkangctx.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gamiqcvjo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gubppociu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/grxftogmd.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gxptdqbrs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gjvwwkyea.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/ginviodvp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gevrivxnh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gekbyvoxt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gjuaibwwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjoddtwcr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gihmlmwtz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gxifzrecp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gxsilxmyj.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gijijovik.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gknlrlxqj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gakbsapzs.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzzmvxktc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gafchjyst.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gzfgwuysb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ghyivikzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcvwgmowa.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ghzmxibso.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gkloxpysf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gyetkwipk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsvpiqbkf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gddyjlufo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gshvzvevx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gfaphmygl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gljzfpmjg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gkimbhacm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gsghnkayf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gcanctorr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/girjmgmjq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gygtdvckj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gssnvttqu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gkolugpck.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gzeefujpx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gklvqvvno.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gweaprxxv.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gsevjmmgd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gdxckzvwz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gakxptkud.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gggvknsur.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gnvrzulgg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ghotvetcw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/giolfjyus.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/ggtoxosvn.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/ghdubylsf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/genrmxpxl.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/goskxssss.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gygdndvad.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gohxwtzlh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gkqelotyl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gstmtyzym.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gmpsxauey.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gimdfglhc.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gvncpjkzq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gpfowpfqs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gcqqjsoag.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gewoyfypl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gckjwixfi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gjcckpypp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpawasidp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gbmlnymyh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gduefjysb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gosacldfa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ghppueulv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gmqxyuatl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gpczcxbnb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcckagwse.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gthmdazfa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqymlzi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gsjrmpsfi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/glipyxypa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gbwrpbjaq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gkykufbnb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gwsjsynfa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gmbdoxfxv.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gjsaswfhe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gxpkchwjm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/glqrsppkc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gsymsxdtr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/guiesmzku.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gjqdtlxph.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gwgtcoyei.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gjgkbcorm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gymnptegl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gcienzcdt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gveutxlvb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gsmdxhmwo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gdilvpwwx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjktzazwu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/grjvsdkht.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gilaipwit.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gihwimjbz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gvuufofad.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/giwoforag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gycnvjzyu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/ghpekqjie.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gfkuwawyu.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gpmqutgto.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gkkqxlatj.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gksnisjsp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gzsodxwoy.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gptqhyhqs.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gwzdvzfcp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gupstelap.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ghbdbnoke.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gakmbgwxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdudxkizt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtyybbiop.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gxnmgnboe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gmdjjjtlz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gmysiecfx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gtemyzeia.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gxkvuflqr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwonsceto.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzpvmlxuz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ggxncpayz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gvxbrckkw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gsnrhtryt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/guqovbphi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gclsdobbf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtqlylvci.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gyplibyca.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvcwrbimu.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/guqywrboq.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gigtmwnts.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gvrblkopr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gemjjsvjs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gslfvakwq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gpagdbzga.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggyeuznci.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gezvxnwtg.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gyccyfvaa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/geobcomza.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gqvrtsmdz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/ghjkcoyan.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/goaumrbht.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/giikbxjas.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/ggnbnobov.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gzwyopnfr.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gemfydocz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gkvfjxkum.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/golomywtt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gijchxtmq.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gapqaxpxc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/guucznzfb.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gjkqolstf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gnpmckecm.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gooqhvbzw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gziwyxncy.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gyozojiha.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjjequs.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gruanuiyw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gjqobctmj.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gquszugdt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqwoqjjvs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gyfubgwsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gcmwbowsk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gunbpbbkp.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/ggiyziaxz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gawewbjus.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gwgsnrzqw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gwaskpydn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gtbpczqru.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/ghturpdzd.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/glltohmdh.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gqhyvmuxr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwcrrleog.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gvegglvka.sHtML


<!-- 参考信息 -->