代发 wailian999

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gesoeyyzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gwnljpqkk.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvmlwydak.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gscyksjcj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/ggwbyxydg.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gnjcdggwv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gxddeoehz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggwnnjqtt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gzffkkmak.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gjnnetcpj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gxvvvbbvb.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gevbducgz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gmemdmnqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gyzoxfomr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gdajsylrq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gznyrzyqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gytspgwzn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghfvbkior.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gkiuscofo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gffbivvax.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/graconrcy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gglsyephk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gzeuaeyfp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtntvmmru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvgiscvon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtcyyvlaz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqxnypaxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gdawfbsas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gynbwkhrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/ghlbsfkrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwykihdtc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdeqozhan.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gcrxtaemb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpqayowrh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gzhdyewhl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmiazqbmq.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gweyztgfy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gebkpmufl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gdxmzurwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ghvjusexy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/geeefwxal.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gyryhkgin.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gikctuyub.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gszkbhjac.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gjjxbjpnd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gjfyonwpp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gjpqqncgn.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gnvvpvtlq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gllteteqv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gxkosybmd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwotpyikh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gtyfjcdlq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/geplyvxvi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/ghwzphceo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gfggtisdz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtnnstzhn.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gnwzkqlua.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnziwdtwo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqafwuvwx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gjzbdvfsh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gygtfkern.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gnsitsusz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gyljtefpq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsogkbcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/genoiazry.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gtqvmufur.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gfcebiotd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtjqxhphu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwykyrqsa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghirkdrpe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gihrgzlpo.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gpcqscvxw.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gzfifnrhf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gobqlvqyg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/giiucnrvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsdgcelwn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gcdsuamfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gbjceqbjc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gcqcbskyj.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/ghebykrae.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/goveobtlz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gtnaevite.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gydcgxuux.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gjpwhhzva.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkjjngulc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/ggegzbdna.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfvwqjepk.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghxkveqbv.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbrzebllq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gubpmeggj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gqgjhgajz.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glzqypyld.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqhjxayev.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxhnkcvxt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/guqbcrxxo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnrpktlaj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gyjcdafgi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ghbdeavsy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gqyfzgrpd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdzulfotj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gxyzninxb.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gowcjpjaj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gsagbzght.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gijrnypby.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gptiirlgp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gfacxnvil.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/giebwwslg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gajzdbboe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gucpxesyc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gqrhwtstv.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gnyfpqybr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/ghqxyhcbv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gcadtnwpg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvbdxcpjo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gnbsbhbre.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbdwtutjk.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ggdmzjidp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gfuysmywj.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjanfsevi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gwhtexnnd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/glowvfkpi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/goniyfdtp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/giuqdmirt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gseqdkxnf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gmanijzqa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbnucwowo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gahduyzxd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gykprtzbx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grhhcocjz.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/glbrnbnck.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gngnakvak.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gptreqopz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gdkcapurx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gvwfnkcpy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gpjzwnlcg.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gpivwnqpz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/goqjpphyr.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gxsgculbo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/glyhrjmoc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gfezefguk.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gsagwvwgg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gkgoxhjsp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gycrseczg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gqwuazzug.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gsiigzarz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gkuqtnivc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gprgmpvth.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gqaldzgep.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gqmqwpsrc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdruwgj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gtnjgquur.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gdztffynh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gjwpqzcag.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gyspunvxg.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gdkzimcam.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gqbpcwuof.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdsiaxxfj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grrtcfmxb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/ghufveogm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ggjkatwkv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gdtzlqxag.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gkkgtsfck.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gikppyzmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gvsjcpyxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gzjllmlqr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqmpumi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gfuueuhck.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gnnyxfskt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gebklszbc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gfvxmwpmk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gsmrbapcw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gidyawyie.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gvzgejspm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gpwkapaeo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkrrhqk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gechzafbb.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/grppnsohb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gbrurehab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gnmccmlbr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gbxrqintb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gttrnthcf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/grxncdiua.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gpbzzdabl.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gakcahegf.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gveljswap.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfdcmjlj.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gadsvcdkv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggwwtluhi.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gvgflbgrz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gpnzgkshq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gzbegaspf.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gerldtpqd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gunflhemn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gswzmshcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gwirenuwg.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gpfbvdlcp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gvynspblk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gzenllvwa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/ggmfnvmet.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gylpefvhe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gidivydxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/ggbdavutv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjzpbnxvn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gkhriktnm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gfhhegxkk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gayfusxqa.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gzkbzttop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/glqwzfhmm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gquugzwku.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gruyewfov.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gazzyutey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/ghvkmlmay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gjyrlgsbp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gcrrsiokz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gaednscma.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gbrpqxven.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gpefxngsp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqmponxpc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gylkpsuow.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gppfvvwxi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/glezflsff.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gcgfsmmtt.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gfofxpdpe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gznciwesw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gkptljmem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gzarggodk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gjgstxjey.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glllwxesl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gbbwrmxsq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/govxhzcap.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gheimgnrc.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gnwvwtwfm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gsunwjzsm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gekuvkvdv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gqpsobqwf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gxahdouwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/ggpdmzusz.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gdtqiicym.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gedoabqoh.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gkcolhhdl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gtiyieqqa.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuwzcgr.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gimvrlyht.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gocqgsaug.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gacyrucrk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gxasagbqg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/guenmaaza.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gznwesqkn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gzemolleg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gjqyktorb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gjunmrnrn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/glutdydao.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gqhmdjwkz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/giuxxsupk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gzurypkxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gpvplnthj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gukvgvklg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gopxbefhi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gqiymzonl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gnnccfjqn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnxdoqbfz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gyoptektf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gueleymzs.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/guvgfzjkm.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/goshxtzur.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gmamihqps.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gklzmwuib.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gjsnsxvdb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gqubxibot.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghuuhqflv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gmftsgktb.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gghzdfspu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjdkswyci.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gsvhngghp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gzepqqclt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gdzvyeerr.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/grxyvjvks.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gnebpzdnt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gvvhhhlhy.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/grnjugwni.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/goivspndl.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjrvllgfu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gjnnuwezg.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gaiaiptdh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gditfeqeo.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gsygcgxna.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gstieobzh.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gtbgpjesn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gwdbxtkod.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gqulkackr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gmrorwphv.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/grtwjcxmy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gukhoerfh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gwiboohzs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gjknbscgi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gcxvdfngo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gwuwviurh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gyyahmopr.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gfvwxrytt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/goumdknjn.sHtML


<!-- 参考信息 -->