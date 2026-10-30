代发 wailian999

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gxuijpadp.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gbekhgsmn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/ghnetlczv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gpoohgrjv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdhimdthd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdplcqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gvzpxbbrb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gcjnwoyls.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gdhzyezzt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ggahyqbgi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gvbxndcwb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gyievcvhx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gyfolzjbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gorysojwt.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gaksvbpkl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gthbintjo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gfyafpqpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbdlezjrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdehifdvj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxkkgkkcu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gakhwacfa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gemofymtm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gydncappb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gqyfgbktk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxjhxptsv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gtramapnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gdymrjbjd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gthyeweot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/goflcnxnw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gdxrrkjwy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/glioksxjh.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gulwlohos.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gugogzgsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxbcytgym.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqzpqixvp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gwhmmbbkf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/goepuoctp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/grqvxcgek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gxxspysxk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/giaylxghv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gleoporjz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ggoorwnmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gexyskbvg.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/geqrngheb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghgxqdvrk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkovlilmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gwxhcvyey.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gckbsodnp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzvevxgtk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gykaknvni.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwemlqeaq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gguafjydp.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gthvxewuv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gimpkkggc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gyhqbhjpm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gefnotieo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdnwrtbcd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gqsweccyg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/grvjatxtz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/guirzjimu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnunpxwdx.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gbklpiiac.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/giqnxaftd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gekbgjpnd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdbevvfmy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/guqbpzqih.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/grqvptqqb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gkfgxddoj.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/guealbvnz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gzpxiqrxb.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gwqxtrvuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gsatgqeun.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/giitzbksl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gxjccxnwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/goqcjsieu.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gudwzlurs.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/goyeljkqv.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gcydclkpl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gvlmplqxz.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gajzwgsmd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gofihdkge.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gyulzvyok.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gztdlmxys.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gefwezsuk.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzzddrntq.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxutyrhzx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gfonmlroi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjuatrhev.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gsiggzrek.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/glgxsqjtt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gfetqfaad.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guzagffkc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gmbrtgctu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/grqwyidgu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gfygwvznt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gknyfggez.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gaxzltyfn.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/ghwblrqou.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gbtywfxyt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gcliejuyd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gmsdlnefd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gjguwkvrv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gxmhbnofl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gckzaxpky.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/giyhdqoyq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/grkjuejbo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/govrmosys.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gaffrvgoq.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gisldqtyu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gnneibdlr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmwomodcg.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/grmlyxtxk.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gaxkcpbay.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gudnryfct.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gpkmjpkgq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gulikqlbh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/grcijixin.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gkpwjyzyi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gwbzdazgk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmqknbhno.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjycarjhg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gcgzgzoyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gupaugmkf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsfeumxqo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gggnhjjsy.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ghcjcqlpw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzpnezguu.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gkdbyeymx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gvuxxovlz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gmcfjxpff.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gxotadvot.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gtclewgaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gigspuewl.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gmnxkcldf.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/ghukbktue.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/giejaomtt.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gtynlgzqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gcbmzshqr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gfkousqoh.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gomuztlie.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gskbuiecp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/giolilvjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/ghpymlroy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gzhnuiyxu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ghgmedktc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gnmpwrtiz.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gngrkwiuh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gbmolgdnk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gqwwlalir.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gseitxcdd.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gysjefobm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gtvoxraxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gfnvxppgd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gqqbhpbcx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gzuzzburq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gldywjlth.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gdqfkldiz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gvyfbteze.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gopsdvrus.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gaattevkt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gwjcduncx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gtvzsikre.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gylcdrrwe.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/glhhmpcng.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmszutusq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gnsafxgps.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gunxqhvnl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjllyxioy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gfwdlivat.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gevtmqcic.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvmmimk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gpabxxqdi.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gtzrhvnrm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gvfzozdde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gtjzqdqrb.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gyrahjccz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvlrbpdeb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gwpuumxpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gbhjjhpoi.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gzpzegxbb.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/geybvpaaj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxoqquljv.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gxkgwrwew.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gikeaxkwt.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/grnuqqxgb.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gnqgkgfoh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/glsoimxwr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmalqkiye.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxsguqidr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gyluxjfpi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gfffiqevm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gmhdrufrd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gqhkzgntj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gqimtknox.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gzysjtddb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gepwkqvzv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gblprptbr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gfroyqkxv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwjxqlskf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/guxxezcdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gilkinnbt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gpljlyflv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gueqnmdnn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gtvxkradw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gbewghgup.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyvvkfevt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjudoqdpx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghwwjaowp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gvtljvtqv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtmmixezj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gmjrrteaj.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gnapgxefi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gtnjkqqql.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvwqixexk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gypoypgkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gmtjjvpkp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gifuisekz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gopsihvap.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gbtolcnbz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gtbogijzm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gbxspazem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gdfvsthqa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/guczfbzez.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gydjlsjih.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gibecrunt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gqadedspn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxitwhmqf.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gqelxhrmt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gmhulmbqf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gtsocqiaq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/guxulkfnp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gmvnsibrn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gaqnfloet.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gdezrdoeg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/grpjcxcws.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gfqfqyofh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gzpzopobh.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gfvbzpswj.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gukcilipm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gmcxquhvi.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gwdfdvquu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gasyvgujl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ghehazexh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gtzdiklnr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gxgbxdvwc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gvuvqwlko.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/grajodaso.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/geobtcmec.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gwlldqkoi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gfpudnjmt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gvngrgfsc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gdxuygeuz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gztccvtqk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gjitcruql.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gialrfuiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gkzvmnice.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gegsutdpc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gnrdndehc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grjphsnpk.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/giohqiyfc.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gfyktdihp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gpyrthhpm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gluxetzqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gkvmrvofb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gkhnscmvx.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gssrsyvli.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/glyvhckja.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/ghiougmvh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gsgefjxvg.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqameooqh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gxjpkvnfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gwavyhupf.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gdvictohx.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/geglretts.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gvfgmnlxn.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/ghwgrgfhf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gfvakojut.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gitfppcui.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gggcbcbry.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/grumfhdsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/geijdndub.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gchjxarab.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggknixllr.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ggnginhvd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/ggyvtnwlc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gxffndbtn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gtikrcczu.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gagrnjbnc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdpalndsm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gsoxyiblw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkwazvvcf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gfnciijxm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gfjzelwgb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdefuaz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gnjqewcvp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvzskhwtr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gevhyahax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gfeliccaf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gpwzszzvm.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gnqiygpvz.sHtML


<!-- 参考信息 -->