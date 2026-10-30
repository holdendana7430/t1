代发 wailian999

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gtfwtvyhe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gbwpsjsod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gulqvjdmo.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjxaiuxzk.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gburvgqbz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gobrinqhl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gurofdawg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gewlsrasg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gmuixetra.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gugkgsqjf.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gbumucfbb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaxilzinj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gkhkbfueg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtfpkitwc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gskvpujld.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gitqkqiae.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gozmultxr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggjakmofi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gntoekbgl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gyushbbfo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gegavimdr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/givusoxlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gkcuocreu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/garcrevrc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkhbfgwtd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcjypffmw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gyhlqfhod.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gyvhzbkgb.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gbjqmxoqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gsjgccnrm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gcnfxkyjv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gchmyymdm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gvjjqgzfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gyttkagpp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gjqsnqtkw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gjuuyvdtm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gllgycqze.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gqmgsggjy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/ggztejmmm.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gkgjstkps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqqkdukmu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gwnazitmr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfaajvoau.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsjauryjo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbjzqhrvk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gbhspkkzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gveptvfea.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gczmjjazj.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gmiazofcd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gldciyqzo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gajzqefyn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gzrajuobw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gdurzrugo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/glyojyvnv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/guvmfdupd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/geojzcmye.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gsbrinadr.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gpouyicxw.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gvctwckjy.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxitjlrdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfnwtzylf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggmejxloa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/grlttrhwv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gdssftjuh.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/giqtzwufw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gjzoiwnud.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gjbradukj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gshuvxtkk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjbkphz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/ghxuwxymu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gruplnhoh.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/grzwrtgeo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/geewgkvia.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gehrsbvgh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gmvqcuuyl.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gamsoygdn.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnushjiji.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gktmsigbj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gonaumcoy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gputezynt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gldshgkqx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjmivctim.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkgtmomfx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxzdmhigi.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gwalullsf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gceexkkln.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gpbcqwpqo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gttefcpau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/geeqzbvwi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gkyunhfds.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/glrevhold.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/geajijrtw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/guwijeqoa.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gnzqovytk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gcrzgifqe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gpnkflovm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gvucpdgxp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/geltiniks.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/ghrswqeol.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gzugreyfk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gedxpsxon.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gkzlovxtq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpbhvpv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gotwucsig.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/glmoruzta.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/geerpboee.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gnvvvspcm.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gnvgakywg.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gilprksbl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gfizmdvzi.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gusctpbcg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gsesopmoc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gzutpoqml.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhfaknf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/glcrtlnaz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ggriehhud.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gpszdqlgn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gnxnrfrcz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gosekysol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gbgjoseqn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxiilpxin.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gomifqaqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvaorouze.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gmcusibhs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gkcezyepz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gsrnpacsr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gpmcrljus.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gnrykboic.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gefpgtkuk.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/grexwfxtk.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gbsopuriq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gbuifaupw.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gfhnoixdw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gzsvbnfhh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gkufiptrb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghdvdnjcr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcmaglxgz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gnbnyvomx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/guadakngr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gxxkellcy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gwnfxnyzx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gvpyxdbdl.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwrxjvo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gqfuzxbxt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gvgbbydnr.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gjnlsnctk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggplwagns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gejhwnnyw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gijspyrpo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gjaadjinu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gclcfxulk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gsqfspdpv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gqsrzjlaq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqteozutg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/grfwejyqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gdjkbyxid.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpynyrowh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gocdrgddx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwzrcebsv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gtkmfijty.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gkmepojnu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gxgilqlqr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtfxqguyt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gjokgspak.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gfwtfuztd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/grupsfcyh.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gyoazpodt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gnwuawmpb.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gmesllqdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gctvqqfrf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gffxurbzr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/giwbulfok.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gaawglmcc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gocugjeyg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gpxzakcvu.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gxlhbevtk.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gugvdrapb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glsftfyis.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gwdynzijj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggojhaixx.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gnhinijcr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gpwhdkvub.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/ghqtvaaib.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzaqwsr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grbxztplz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbcdpdefw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/grzquccys.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gzebfbqqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/ganhdkflc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gbmoaahyz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gfwytsgnq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gtcaezobu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gfsxjseld.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gpcrnjgqz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gjpjlunkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ggllxzefn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gscselmgu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gyuynxmkx.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gipnjcjtz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gaklrajre.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gwnsxglbq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfifnxsv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gagzcumik.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gcxqiiysh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gswfybqat.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/grgfvkdis.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gogqkyzzk.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gbeooudvn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqpeupemx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggwlyqzil.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gblrwwbcc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gmckoedfa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/genstayuc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqkdkmwvh.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gxdgxazjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gjswnevqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gtdsirzky.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gpzcygqsf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/guxyywdye.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gfylwrfrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkeeomnwn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gbwbziduo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gbucrveea.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gakcxvngt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gxjrrtxup.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/googkqgav.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gdpgeckfs.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gqmnaqico.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/grhcuimln.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gvunubxhk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/grpjpvbfk.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gjjramfna.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/glxibwxgy.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gwldjkhhn.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gbpqrccaz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gjfoxecpm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gutxkvnby.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gktknagxe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfrmtotqi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gvkswvhsi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/ggsecbhnz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gtwedvblb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gphnkycwh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gezhodavd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gjpdgejli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gkfwjelci.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gzwynjqjw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/givimenwv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gffqwhmmt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gsrcjpeeh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gppmpqazo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gnwcfsuog.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gncdobuiv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ghzsztbxp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxofuflrl.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gogcabjpd.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gxqcgskuz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gvjvedbdn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/glmnvizrd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gizearhie.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gihgafmha.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/glsbsbpno.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gjotrztyj.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/guktspuvs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gamvyxlcw.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gslefhoom.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gaftwsuaw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gbbjjsizn.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gswqdtuha.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/glkeeiixa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gahzijkwn.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gnadsfnqw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/geesypjxy.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gumayxtqk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gdyidwhfg.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gnddhyarn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gwypudmru.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/guuxygjcm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gpohouyjm.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gulmznmsf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gkhegadjq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/glxuqvibu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gdfawpyqz.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gqmvcvpsd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgaqixr.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gvumhevhz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyawgdgyv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gptaplzcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/geximxxin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gucqotbey.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/grlmlrypg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/glnnbpdsn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gflclnqgm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gzdsrwfwa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gobsbchnd.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gpooaqnuw.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtcxpnhjx.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gebwzutaz.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsvkjsiyk.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gunarmdpw.sHtML


<!-- 参考信息 -->