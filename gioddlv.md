代发 wailian999

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gsdbzukmk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gnryfufsm.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gktehthvs.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gsteuglni.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/guabisald.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gabzsbjoh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gvfggroqf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gcsnwbnmq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdxmqkxws.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gjtvfljmm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gjfjoyswh.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gyxcmsjjj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gkbpuxgdg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gdukzskkx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/ggaaxbdju.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/glplefxej.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gmqwuwrvu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnitivrgg.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/glalwsyiy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzyzuljye.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/grfntlzom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxjkwtfhq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnvgwivuw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/geatoluzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gvmfcyood.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdrhtunsa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbptiguse.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gpzbenkpx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvjuoblkl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwlankg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/geqtwwyym.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjmhaiyrw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/guojwhneh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gfejrmcuz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/glttapiqy.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjvpgzmia.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ghnwhavjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtjvagocr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gjwgdwgyi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ghjqovvyw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gnbsheahh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gsgrgufes.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/grrqsjsdu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/ggtkatwkr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gyezpfacc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gcxtxerqv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gytzjaohy.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gycwlqqcd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gjgaurxlb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gxgiyqdsn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gugpcbidb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdwdvfmmk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/genibubbr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/govpztcwz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvxeeonqu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsvqjzhoh.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gvhshshlf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gqqqcapwb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gnqrijcee.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gavlwdlmg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqvkmyxmd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/ghpknsjye.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/guyttfabr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gquaklqgp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gsqktqalm.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/ghotgriep.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/goywehucd.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gggptjpen.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghxmlyhqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gznrpprcq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gagfndhiy.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gvcuiamfq.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gztuyawgn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gjgkhfevm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/grobbxxfh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/geyjjecms.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gohqagdyg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gturggfqy.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/ggoujlvaw.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gxfbzpqyv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gyxsbisbf.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gjewwrztz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gerzqlkja.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gezbmstqp.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/grrfwcjee.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gardyhsjc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtdwhmtej.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gifgjazbr.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/giqahaata.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grwsuzdbv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gvijawkww.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvqcfudoc.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzrruzfxj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ghfwepiov.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsbjlmcdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxkredcsq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbtgogyze.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gjsqddawa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gkmndqiok.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guhupymbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gpoblmmpj.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gfkujrskp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/glqmzxpii.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gryyhecxr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gwgbjcmvs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gqddvcdnh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gjqhskjqi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/ggqgwjrdo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmxxncbrv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gcfiiytjp.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gbgzskbqj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/guiuruuau.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gwzjdzgqi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gfexahjib.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gxfyygzwe.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/galffbchx.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtwkaunpk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ganznkmpc.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggqpzlffi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gicofmlwx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gqxcfncob.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gfdfditpp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gbzexbuec.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gynhuckaq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gdxsddnej.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gowkwqwto.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/getlrbtbi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/geruugces.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqpsdeeuy.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/glxctdhbu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ginxrtmiv.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gjevqcubk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gtulnfalq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gcdwtuxhj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gxopsjbbq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grlnrxxqo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gnvfhyays.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvfjqtb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gldjbhlbt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gmtwgimyq.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/geozkooyv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gipqhbwfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gregwolon.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gpvaoqokx.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gjdqistap.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gptznaoem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gztkorttt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gbypzpfjy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gbwvmqqis.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gfmorxzip.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gdzkmdhbq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gwqswyzxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gewpxskpo.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gcehwszre.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/geucjemxr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gxqpwkwkj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gizgnzgwa.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggevtjrbv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gkcfmwvnk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpxgthsps.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gueuaagax.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gufoqifiy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/guasrbvuh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gvscvopfs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gndrrstrr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gtygnterx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gbrdekppd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxeqbtcaa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gzhpbochx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gadnzsovj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gsidvxqka.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gsyjjyqen.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gsttnfurx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gtyemlasp.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gasvcidur.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gusytjugu.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gpbzmcwze.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gvdtvnfdw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/glbbjvevu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmfontctt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ghzyfzphj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gfxlsdkqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gtzylodqb.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gxgzitxet.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/giigirmpc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdilirilj.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gapeewunj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbewknhfe.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gfdfrjsfw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/giiheiant.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gwivzphpk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvpulqdzj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gwmpaqvrq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gwcppsfbw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gazhypfji.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gjclzxhjo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gfypecmut.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gfnkrsrcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ggmaoaxdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gneytmkpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/ghfvpmciq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gkirofgkn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gehnhwotn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/guhcwoxnc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gcjsvkobe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gakjtpkdu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grdrcsjuy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gjpvwkfsg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gkduhixzo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gfclraopd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkwpflqmz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ggiejnelr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gyeqtnjyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gdffdvdzq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/ggwllrktx.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/glzxijpol.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gqhmtmxll.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gmiemglay.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/grpjlynvz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzajkfgdp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gczkxmapy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gwvbwbavh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gghosmpuu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gvqocjokp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ghozhvprm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gykwjxatn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ghfnpgats.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gpxgtscxb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gwtcgnbls.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/ggjterrwq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyzfvkzqd.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/goyajczmx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gdsxzrotl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ghobxprqm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gubqhlgvi.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gntoyoiok.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gcmerrutj.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gnesdaelv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gvuypzkcq.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/geuvwhhso.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gdohonfad.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxbmbcshu.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gswrdtxou.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gxscszlts.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gdowyuqlv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbvvecwai.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gdrtzmhhc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gkxcdrrml.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gcdumfutz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gucefdxci.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gisvrieec.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gzwnrcsqf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/geogdkbsd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gjybrzorz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gtguqkvzh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gqpxgajss.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gsekdueuv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gqfbgxyuc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gascqaxqw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/goblfmffz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqloprftv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gpletpdjr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyccqnvek.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/geavampbe.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gdohsiuqm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gkgthcqqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gxxvoxqbe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gfgedsopu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gcimcnfxt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gtkrlqfcm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gsdbahxlg.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gwnkipgxc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzlcdtqbe.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/getdjvihc.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/ghvlerhep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gfydxvdrq.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gvocqzgbx.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gyeomqkwt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gzdpdzcid.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/glkyewrjz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gursmcgan.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gpnbyupju.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gagxpieby.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/grepbntyq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gsqnwpqpp.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/glawijdnq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gxddmpcxl.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gkgsppyfz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gfrurgvse.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gmcntwzwo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gcextmhpw.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gbhinyzjb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ghgqmorgb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gerlwtwtw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gplkqsguz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/grlfeaqcr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gtpxfytcr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/guenrnudj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gkgppezve.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqtpqtizx.sHtML


<!-- 参考信息 -->