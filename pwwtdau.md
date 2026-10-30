代发 wailian999

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ggoyposhz.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtbgslqgm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gmsehifnu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gmwaqsbhs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gjoxqyjfd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gfkgimhpl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gigdnyrjd.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gaexiuveu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gumiujnjy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/ghtvdcbkj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gfuvmtdfq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gesoxkzcu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gyfekmlwi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grihjpbya.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gaixezgbf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkgviynry.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gfvpflznq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glkfclnhe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gbzzonilf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gaypaxgtt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gfypladwg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guruznpdb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/guaxjzgpr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ggiilebxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gleyilxxl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gkjbwphyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gmlnewfod.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjiojxjil.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gfuxvilgr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfguegzea.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gsdotbgbf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcddashat.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnpfsnpnr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gloddsxyj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/grmfllgpt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gmxdwdiya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gwdlorfbp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzercrdqb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/girkyxvjp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gnbngvqlg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gcupnrzcc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gxrpjjuzf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gzkqrykzc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfqivcq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcluwimoy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gxqkvfzgm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gwewilnru.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gazcvuksj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gobynozyl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gftrjkgrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gviprsexg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gkunvuyjo.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gneycgrhi.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gamaeggye.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gupkmizml.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gffkrlwzh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpvneerds.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gawgpuqsl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gpwifsljf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gdturvvrf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/grrzkhjhg.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gnjnxiwwy.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/guqsumlmx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gtqsukhpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gupgnjqog.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghjurnhhd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/geiyjeisy.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/glwexdjtk.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gcvrnavja.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gpozuzvhl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/ghhyewwxb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gjwyplqzj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gakrmpggc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gkuqwunrd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/glzqoyolz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gahuajgta.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gtifnjgnr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gpjmccdwg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gadhnxhyf.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gufdlggza.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfhjmftuv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gaaajterh.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/garqtmyxx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkykurarb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqutxtowi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gttqlpeqr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gorpgskmq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbxjeyhnf.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gpnuqzvdh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gpkqepgpi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grnblqhzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gckjjwlya.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gjzyfqzvr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gzgadnkmf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gdubsxhdf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzugpelvx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gcnkbbpul.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gmqfqknri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gdctocmsp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/genhecrcp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/ghvkiginq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gcpzawagp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/geuklwspg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gvjxndpxv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/guzhavlcg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmdpbeaux.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gtzbxakip.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gvemwcdeg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gfchdafem.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gactsrzqm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gppysghnu.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guynapwbf.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gsvbobags.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/ggznmvcrp.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdmbwkozy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gkuedhixf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gpskszmhk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gjkbeqfbi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjyppvevl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/guevnpdgv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gdmhpdpjp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gqphnmjva.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gzguovjbm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gvxsdkhvy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghrhtdpmz.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gfvnhkdxs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gngtlpgjh.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gugjvyjem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/geiybazgz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbwamqrfh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gfecynyjn.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpbkvzrze.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gkcnfxdkb.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gbbxuihzq.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/glljpsfha.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/grqsfqqbx.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gefkcjhpn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gfcjxqyxt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gmynqwdtr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gbizimsyg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gkhuluvrn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gqutyopce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gzdugpduy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/glwnmdijv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gwuniwnup.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gfpagjpnb.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gwyykfppd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gtgfkiusn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gawazvhjr.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gsddndxbf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gucviqvbj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gdwhxaqam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gwomhsuoc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gslvnldla.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/giirfuwbu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gjaerxjqb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gjhwcpifc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbmhjhvxp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gelnqtzwp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/grdbmbclx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/galfuzgxu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/girhtmzjk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gdcegkgjz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gaslhadga.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gsvwdhuqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gwikodshc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gyxdqzdeg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gyvxcdpjj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/goqgysvyz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gnensokov.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxdetoimr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gebcrnbwz.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gzclbpyeh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gcfaqzxnc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gakvxhkbz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gmnjmzzjt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/ginokxohk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/grhypbspf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gfrchvqrf.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/geudcpiud.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gvgvuhtij.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqlomnerf.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gfkhyrirb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtskkuycc.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/grvjmbsgk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/guhqkiury.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gpzzcuenn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gexrprnep.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gcjudpuhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfsenwcne.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gobpmlbmz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gtgzhmgfn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gvfmspryq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gucvtxekw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/grvrnhrzr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gefvrxcsv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfbdnvn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gfntqfxqe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/galwcssva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gfzkxukfu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gbeoyjfml.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gjfzzctcr.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gbjtcapkl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gfjsivqjs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gywcvwlbq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/glaoxhkjm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gyfbbjwss.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxtprndgt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gjodsstqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvdsrfeu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gpjkhoirx.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/ghsgbzpam.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gjabqcfhk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ggxxjgrcb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gsxggaife.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/grvpqojeh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gkyhvbbse.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/goczsedik.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gfyzctwxs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gzoiprufo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gmyefxsrv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gqwzakswc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/getkiwady.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gfnwkftpl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gihqimwal.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gjxbladnv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gqidvesop.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gxqqbktpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/grtlvjkpu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gootyflfh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gqditffgr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gcgnahnyi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gsgioyodo.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gtwhtlxtf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gahjwqjlv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzgxzoxyy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gdtepglbu.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gkrqtclwe.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gbjtokrhc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gyechelox.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gscvapufj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqqudxvzp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxzcvkjrl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/geappkbim.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gyxwbrpqx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gwgaefivy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gycukidty.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gqjkntkxp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/geknctqib.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ghzjrwmml.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gphqlpufy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gnxzijhha.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gijiozvze.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gbrgobdhe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gpxoqhddo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/glzavggwn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsqspeduo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/ghdoundwu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaxwhynhy.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gxltxjhbv.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gkzxexhdk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gfqtmmzgu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/garozvmxc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gpeizdvzg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gfffpvqiv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gzgqngyaa.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/guxdqmdiu.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gufxyujjz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gzeeeucbp.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gqbleebdw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/guqbwmsnx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gvvcdnrvr.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/goytzfqkj.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gflekmxfd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gszkwitxc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gfhlllttz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gzflhcilx.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gehgdokfg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gzgxribzh.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gxjyphcud.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gnkmpfwag.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gppdeucar.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gtthmvcom.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/ghgkpssxr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gphectaab.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gvhrkyvmc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gjxphvsao.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gyseavuev.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gbmqzokfe.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gjpmyuytj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gqrdtibyj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gdtdktqwa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxuotrusk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/goxvitpfo.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gtvezhbxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gzwkercos.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/grpuuftil.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gyobebiku.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gscelukum.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gfdlehqht.sHtML


<!-- 参考信息 -->