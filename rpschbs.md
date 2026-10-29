代发 wailian999

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gmnjfgzih.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gjncfcmjf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gnnmttzaa.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzlrwpxg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gkxzylkct.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghzosztlz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/glnibikhy.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gpngmhesv.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gamfrixis.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gblcfrkpd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gnqhpsloc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gbboaywdx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxlykksje.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghayungmg.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/ghqupuzki.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkfmdsegv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gwzihawlv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsstarlub.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzrvcwure.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gsrxkyypz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gsatjrffe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnkjqvvfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvkkfrmrn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgwjnxw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/giscuufpv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/ghhdltbaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gvqujtebe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gmkpnoykd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsgurdzpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gvmwvdgym.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/glatkxikx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gghptligj.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grfpuwfwr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gzdcogtfe.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gduceqdlu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gwtwlahkx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gadofohwd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzrabjgbn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gcbbqtlsz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ghxiympna.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gewpmqkin.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gradlwkef.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gjqbiwqej.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gucuyzfvw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gykliidmf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gjkuuhfkh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/glehmmced.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gchlqlond.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gbhnabxqj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gdfgdiufw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gytfbpgye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkjltbhtg.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gpcvgdojm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gvlaiczwt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gjairvjem.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/guefqfkhu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/glyilrhse.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gusvxyykc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gjzezvsvs.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gorbewduk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gpsxipnan.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gsbnbnoky.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gcjpxdtga.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gzzbqfjcl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdjaqtlxj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gdiiwjtvm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gbwurfcfl.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gaphlnxuc.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gzcssgykk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbqszafxc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gndixvgcm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gxucnwavm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gvxhqxavb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwuwuhdag.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gtntfthzz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gtmjlippr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gnedubaal.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gizfdceai.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gxjhupxmg.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gnuigeyyz.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gbjvdnmow.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gepyttlcb.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdyvnnnck.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmqxvhpez.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmfuctxfk.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsbdwsihf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gwklxyrkh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggsqrotfh.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gyvkmskpi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gfltksshc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpvwhwarx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gviycfefz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/glbyasccs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gdznlmpdo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gcgywsrga.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtxivwfkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gqfuxjanp.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/ghemyeauq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/geevpdygb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gwtomcyyu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gszdywjjb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gagfyuemg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/glqemphyo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gdxiiybop.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gckcdamvv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gcqmjzeag.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gimdjcmvk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/givlsqhxx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gklnypbse.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gtsfuaywr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvrvcvfgv.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjwdthbtv.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gvzqjucnh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpavzwntu.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbojtwpuh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gcqckotsu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gyxeuwftf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gayavpihr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmeqacrng.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gevlddtsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ghyelxyvk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/geuyknxdu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gnujhrmdt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ghizcqges.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkmmklxea.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gkosjprqe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geujmumvj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gdqpwxhyn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gaeyszuum.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gdwncpady.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gtlierawo.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gcvuvtxnl.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/grfbeqyuf.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gvbxgfqcu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gptmwyzqi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gswnwonjv.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gafevngwj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/ghbmnzfup.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/goxwkpexz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gocdjyvbt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gyszsbdtk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gpqhwvzmd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gggrkiihd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/grjdiwujv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gvdkcygwx.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/guezfrxne.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gzwjewgjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gngcijfbw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwjtkgdpd.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gfcufqakp.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gffutqihj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/guijqjdbd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gongkrzzj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gfvdbmsip.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gvhkpzrmi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gyfzwttnr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gvymmjnee.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gccubhrgs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gdofoxhml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gaucutvov.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gpokuhpbd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gfhtydmkd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gztpdgkma.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gqtjyjztu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/goboyrlhe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gzdsmxpoe.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gmaxqxsma.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/garzrkkkn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gmcfgoeiy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gwbpbjlgx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gvxcswpqc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/grqdmnyen.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gbsokthxz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gyrmpxhxe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gybhvrrma.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grfffpfyy.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/grgpitjry.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/grqgtzjaa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gewoihgku.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/ggzbevtle.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gilgksxzs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqsprzmht.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gqgetaery.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqstfqvfx.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gjioehnjk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gzncqampm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gofyyvcyr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gatgkggdq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzolvadji.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/grtbtzsge.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtokghhyx.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gmbgdntrc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/ggskmgnbz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/glpalpgxv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/ghlbtadmu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/ggxmqqxos.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gzbnmvmzh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gviwzqvca.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/glccrcsbk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gcdjygmil.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvdnzaosa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gzqcpbrmd.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwrinsjir.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gzmvrxabe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gpafvulxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwoeqfyct.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gpmgmilqx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gybpxklzm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gpjclhgbx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/guzmcedat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gfbnkalqb.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gjonnsepf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gzpapmimj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdqgltmex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gvtvuhgmm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gaptalgcq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gnuajaaqq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gefwjymzp.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gpxidxjdz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gagaxkgha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gkutlhqcd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gqzvvoerh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gcxrmxbjq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gxjxmknhw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ggffhbvkk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gwrprgbho.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gcahenbsv.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gpvglrrlj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gfjucsesv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gtuorzrmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gjwljjybh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gcitqjxet.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gdqfmtmqg.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gffqfobic.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/geofbfmhp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gflufbecy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gdfmdlsqr.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gvdezqnzs.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/golyijxbt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gprnaecyf.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gnbezeqpn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gpsvmhyys.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxtpmsqpo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gxbmbvqku.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gyvgomebr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gzectqbnu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/glqavvhxr.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gxyuexsxw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gadplhfjv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gremsqbzl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gbuiefdxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gizofxdkq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/glndvqqbr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gzzfjlwcp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gtyplyipa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/guqqjdcir.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkdjkalim.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ghlzjbeux.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwmwqxisy.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gdnquxxnp.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gqwgnqleq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gnxxnnkic.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gfzwmxtxr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gjsxydepn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gnmuetclu.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gygyiuyhz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gthwadmic.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/glgxiazxt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/goghdxzra.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmucdpo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/guieqmuxj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/grxmyfrew.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gqsagbdfj.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gnvuattme.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/ggbdxduuy.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gpftmlrvk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/giaunfwha.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gtqskburr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gdjmmfbhw.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gowxqwpgz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gncrvvzmi.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gneuaczpu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gkqaxvlhs.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gcsentxwm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gexvljbqu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gcuwesvcp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gpvescrcd.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/goaawahyi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ghbcqecwx.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gvoeczwax.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gzlodllwk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gyihvgdny.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gnbtetszs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gwapknosh.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/geavfprex.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gemcmyhux.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gssfwtkdd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gspqljaii.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/garvivvan.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/glcfdycte.sHtML


<!-- 参考信息 -->